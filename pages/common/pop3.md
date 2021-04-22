# POP3

> Post Office Protocol used by e-mail clients to retrieve e-mail from a mail server.

- Connect to a POP3 database running at a certain port:

`nc -nv {{addr}} {{port}}`

- Your user name for this mail server:

`USER`

- Your password:

`PASS`

- End your session:

`QUIT`

- Number and total size of all messages:

`STAT`

- Message# and size of message:

`LIST`

- Retrieve selected message:

`RETR {{message#}}`

- Delete selected message:

`DELE {{message#}}`

- No-op. Keeps you connection open:

`NOOP`

- Reset the mailbox. Undelete deleted messages:

`RSET`
