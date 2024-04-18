---
title: Mem read in x86 Assembly
slug: mem-read
draft: false
date: 2024-04-18T15:07:36.885Z
---
You have to initialise mem read with an address.

```
mem read --size 1 --num-per-line 1 --format x --count 20
```

Subsequent calls to mem read without specifying an address will keep moving forward, based on the count of the previous mem read.
