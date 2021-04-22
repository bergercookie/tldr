# SMTP

> Simple Mail Transfer Protocol Cheatsheet.

- Authenticated TURN:

`ATRN`

- Authentication:

`AUTH`

- Binary data:

`BDAT`

- Remote content:

`BURL`

- The actual email message to be sent. This command is terminated with a line that contains only a dot '.':

`DATA`

- Extended HELO:

`EHLO`

- Extended turn:

`ETRN`

- Expand:

`EXPN`

- Identify yourself to the SMTP server.:

`HELO`

- Show available commands:

`HELP`

- Send mail from email account *MAIL FROM: me@mydomain.com*:

`MAIL`

- No-op. Keeps you connection open.:

`NOOP`

- One message transaction only:

`ONEX`

- End session:

`QUIT`

- Send email to recipient *RCPT TO: you@yourdomain.com*:

`RCPT`

- Reset:

`RSET`

- Send and mail:

`SAML`

- Send:

`SEND`

- Send or mail:

`SOML`

- Take an existing insecure connection and upgrade it to a secure connection that used SSL/TLS:

`STARTTLS`

- SMTP responsible submitter:

`SUBMITTER`

- Turn:

`TURN`

- Verbose:

`VERB`

- Verify:

`VRFY`
