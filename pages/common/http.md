# http

> HTTPie: HTTP client, aims to be easier to use than cURL.
> More information: <https://httpie.org>.

- Download a URL to a file:

`http -d {{example.org}}`

- Send form-encoded data:

`http -f {{example.org}} {{name='bob'}} {{profile_picture@'bob.png'}}`

- Send JSON object:

`http {{example.org}} {{name='bob'}}`

- Specify an HTTP method:

`http {{HEAD}} {{example.org}}`

- Upload a file using redirection:

`http {{example.org}} < {{path/to/file}}`

- Download a file using redirection:

`http pie.dev/image/png > image.png`

- Have a persistent session across requests:

`http --session=logged-in -a {{username:password}} {{example.org/get}} {{API-Key:123`}}

- Include an extra header:

`http {{example.org}} {{X-MyHeader:123}}`

- Pass a user name and password for server authentication:

`http -a {{username:password}} {{example.org}}`

- Specify raw request body via stdin:

`cat {{data.txt}} | http PUT {{example.org}}`
