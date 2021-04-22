# perf

> Framework for linux performance counter measurements.

- Record at 99Hz, across all CPUs, generate callgraphs:

`perf record -F 99 -a -g -- {{command}}`

- Record with dwarf symbols:

`perf record --call-graph dwarf -- {{command}}`

- Collapse trace outputs:

`perf script | stackcollapse-perf.pl > {{out.perf-folded`}}

- Collapse trace outputs  with Inferno:

`perf script | inferno-collapse-perf > {{out.perf-folded`}}

- Generate an SVG to visualise:

`flamegraph.pl {{out.perf-folded}} > {{perf-kernel.svg`}}

- Generate an SVG to visualise with Inferno:

`inferno-flamegraph {{out.perf-folded}} > {{perf-kernel.svg`}}

- Display basic performance counter stats for a command:

`perf stat {{gcc hello.c}}`

- Display system-wide real time performance counter profile:

`sudo perf top`

- Run a command and record its profile into "perf.data":

`sudo perf record {{command}}`

- Read "perf.data" (created by `perf record`) and display the profile:

`sudo perf report`
