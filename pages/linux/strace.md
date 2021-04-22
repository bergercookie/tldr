# strace

> Troubleshooting tool for tracing system calls.
> More information: <https://en.wikipedia.org/wiki/Strace>

- Start tracing a specific process by its PID:

`strace -p {{pid}}`

- Trace a process and filter output by system call:

`strace -p {{pid}} -e {{system_call_name}}`

- Trace a process, child processes and all threads:

`strace -f ./program`

- Count time, calls, and errors for each system call and report a summary on program exit:

`strace -p {{pid}} -c`

- Show the time spent in system calls:

`strace -T {{program}}`

- Trace specific system calls:

`strace -e trace=open,read,write {{program}}`

- Show the time spent in every system call:

`strace -p {{pid}} -T`

- Start tracing a program by executing it:

`strace {{program}}`

- Start tracing file operations of a program:

`strace -e trace=file {{program}}`

- Print a histogram of the number of system calls and the time spent at the termination of strace:

`strace -c {{program}}`
