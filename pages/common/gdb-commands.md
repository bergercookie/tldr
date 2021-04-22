# GNU debugger - Reference Page

> Debug executables
> More information: <https://www.gnu.org/software/gdb/>

- Connect to a remote gdb session at a port PORT:

`target remote :{{PORT}}`

- Show all breakpoints:

`i b`

- Delete breakpoint by ID:

`d {{1}}`

- Watch a vector in a (gcc compiled) executable:

`watch myvector._M_impl._M_finish`

- Show machine registers (except vector and floating-point):

`i r`

- Show all registers (inc vector and floating-point):

`info all-registers`

- Show backtrace:

`bt`

- Print a variable in the designated format (same as printf):

`x/s {{$rax}}`

- What line is the instruction pointer at?

`x $ip`

- Where is the stack pointer?

`x $sp`

- Display a variable every time the program stops:

`display/I {{$pc}}`

- Show help page for a particular class:

`help running`

- Start debugged process but stop automatically on main:

`start`

- Step one instruction:

`si`

- Add to the stack pointer:

`set $sp += 4`
