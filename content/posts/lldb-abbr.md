# LLDB Abbreviations

| Command | Description |
|---------|-------------|
| add-dsym | Add a debug symbol file to one of the target's current modules by specifying a path to a debug symbols file or by using the options to specify a module. |
| attach | Attach to process by ID or name. |
| b | Set a breakpoint using one of several shorthand formats. |
| bt | Show the current thread's call stack. Any numeric argument displays at most that many frames. The argument 'all' displays all threads. |
| c | Continue execution of all threads in the current process. |
| call | Evaluate an expression on the current thread. Displays any returned value with LLDB's default formatting. |
| continue | Continue execution of all threads in the current process. |
| detach | Detach from the current target process. |
| di / dis | Disassemble specified instructions in the current target. Defaults to the current function for the current thread and stack frame. |
| display | Evaluate an expression at every stop (see 'help target stop-hook'.) |
| down | Select a newer stack frame. Defaults to moving one frame, a numeric argument can specify an arbitrary number. |
| env | Shorthand for viewing and setting environment variables. |
| exit | Quit the LLDB debugger. |
| f | Select the current stack frame by index from within the current thread (see 'thread backtrace'.) |
| file | Create a target using the argument as the main executable. |
| finish | Finish executing the current stack frame and stop after returning. Defaults to current thread unless specified. |
| history | Dump the history of commands in this session. Commands in the history list can be run again using "!<INDEX>". "!-<OFFSET>" will re-run the command that is <OFFSET> commands from the end of the list (counting the current command). |
| image | Commands for accessing information for one or more target modules. |
| j / jump | Set the program counter to a new address. |
| kill | Terminate the current target process. |
| l / list | List relevant source code using one of several shorthand formats. |
| n / next | Source level single step, stepping over calls. Defaults to current thread unless specified. |
| nexti / ni | Instruction level single step, stepping over calls. Defaults to current thread unless specified. |
| p | Print a variable or expression. |
| parray | parray <COUNT> <EXPRESSION> -- lldb will evaluate EXPRESSION to get a typed-pointer-to-an-array in memory, and will display COUNT elements of that type from the array. |
| po | Evaluate an expression on the current thread. Displays any returned value with formatting controlled by the type's author. |
| poarray | poarray <COUNT> <EXPRESSION> -- lldb will evaluate EXPRESSION to get the address of an array of COUNT objects in memory, and will call po on them. |
| print | Print a variable or expression. |
| q | Quit the LLDB debugger. |
| r | Launch the executable in the debugger. |
| rbreak | Sets a breakpoint or set of breakpoints in the executable. |
| re | Commands to access registers for the current thread and stack frame. |
| repl | Evaluate an expression on the current thread. Displays any returned value with LLDB's default formatting. |
| run | Launch the executable in the debugger. |
| s | Source level single step, stepping into calls. Defaults to current thread unless specified. |
| shell | Run a shell command on the host. |
| si | Instruction level single step, stepping into calls. Defaults to current thread unless specified. |
| sif | Step through the current block, stopping if you step directly into a function whose name matches the TargetFunctionName. |
| step | Source level single step, stepping into calls. Defaults to current thread unless specified. |
| stepi | Instruction level single step, stepping into calls. Defaults to current thread unless specified. |
| t | Change the currently selected thread. |
| tbreak | Set a one-shot breakpoint using one of several shorthand formats. |
| undisplay | Stop displaying expression at every stop (specified by stop-hook index.) |
| up | Select an older stack frame. Defaults to moving one frame, a numeric argument can specify an arbitrary number. |
| v / var / vo| Show variables for the current stack frame. Defaults to all arguments and local variables in scope. Names of argument, local, file static and file global variables can be specified. |
| x | Read from the memory of the current target process. |