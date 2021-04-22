# systemd-cat

> Connect a pipeline or program's output with the journal.

- Send the output of a program to journald

`echo "hello" | systemd-cat`

- Run a program and record its output to journald:

`systemd-cat ls`

- Send the output of a program to journald - Add an identifier:

`echo "hello" | systemd-cat -t {{"myapp"}}`

- Send the output of a program to journald - Add an identifier:

`echo "hello" | systemd-cat -t {{"myapp"}}`
