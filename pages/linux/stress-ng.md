# stress-ng

> A tool to stress test CPU, memory, and IO on a Linux system.
> See also `man stress-ng`

- Spawn enough workers to fill all the CPU processing units and stress the CPU for 20 seconds:

`stress-ng --matrix 0 -t 0.3m`

- Spawn 2 workers to stress test IO and timeout after 5 seconds:

`stress-ng -i {{2}} -t {{5}}`
