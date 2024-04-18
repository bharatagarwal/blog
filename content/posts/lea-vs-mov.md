## The dilemma

In x86/64 assembly intel syntax, for a long time, I've been confused between the load effective address (`lea`) and move (`mov`) instructions.   

I've been imagining was that `LEA` has been doing some magic, taking contextual decisions based on whether the values inside the square bracket are addresses or naive values. This seemed counter-intuitive, seeing as assembly is supposed to be simpler than most languages.

## An example

Say, you have the value `0xffffffa` in `rax`.

How do the following two instructions differ:

```
mov rdi, [rax]
lea rdi, [rax]
```

### mov rdi, [rax]
This is equivalent to,

```
rdi = *rax
```

### lea rdi, [rax]
This is equivalent to,

```
rdi = rax
```

Now, the square brackets notation, `[]` indicates that the operand is an address.

We can do things like,
```
[rax + rdx]
[rax + 4*rdx]
[rax + 4*rdx + 5]
```

Whatever the computation, the meaning of rax and rdx does not change, whether we're doing this for `lea` or `mov`

Some rascally developers might contract the following operations

```
add rax, rdx
mul rax, 4
add rax, 5
add rax, rcx
```

into something like this

```
lea rax, [rcx + 4 * rdx + 5]
```
Thereby reducing the number of fetch, decode, execute steps. Furthermore, the fact that it follows a pattern of

```
a + 2^b * c + d
```
enables it to have a more specific path than those individual circuits.

The fact that lea has its own circuitry means that it can be run in parallel with integer circuitry.

## The logic still stands
Even though we're gaining all of these advantages, at its root, the lea instruction is computing a value, and storing that value in a register. The mechanism was designed for computing values, but there's no sense of a 'type' here. Any value computed inside the square brackets is considered an address, and lea simply stores that value -- it loads the effective 'address' in the source operand.
