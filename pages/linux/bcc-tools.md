# bcc tool suite

> Tools for BPF-based Linux IO analysis, networking, monitoring, and more
> More information: https://github.com/iovisor/bcc

- See the kill signals send and received by the processes:

`killsnoop`

- See the kill signals send and received for a particular target PID:

`killsnoop -p {{PID}}`

- See the exec calls being made:

`execsnoop`

- Snoop output from a pts or tty device, eg, a shell

`ttysnoop`

- Display kernel tracepoints or USDT probes and their formats:

`tplist`

- Display kernel tracepoints or USDT probes of a specific PID:

`tplist --pid {{PID}}`

- Display kernel tracepoints or USDT probes of a specific library/executable:

`tplist --lib {{/lib64/ld-linux-x86-64.so.2}}`
