# hydra

> Online password guessing tool.
> Protocols supported include FTP, HTTP(S), SMTP, SNMP, XMPP, SSH, and more.
> More information: <https://github.com/vanhauser-thc/thc-hydra>.

- Start Hydra's wizard:

`hydra-wizard`

- Guess phpmyadmin admin page credentials:

`hydra -e nsr -f  -L {{path/to/usernames}} -P {{/path/to/password/list}} {{target}} http-form-post '/phpmyadmin/index.php:pma_username=^USER^&pma_password= ^PASS^&server=1&target=index.php&token=&token={{token}}:Cannot log in to the MySQL server'`

- Guess wordpress admin page credentials:

`hydra -e nsr -l admin -P {{path/to/wordlist.txt}} {{host_ip}} -V http-form-post '/wp-login.php:log=^USER^&pwd=^PASS^&wp-submit=Log In&testcookie=1:S=Location'`

- Guess SSH credentials using a given username and a list of passwords:

`hydra -e nsr -l {{username}} -P {{path/to/wordlist.txt}} {{host_ip}} {{ssh}}`

- Guess Telnet credentials using a list of usernames and a single password, specifying a non-standard port and IPv6:

`hydra -e nsr -L {{path/to/usernames.txt}} -p {{password}} -s {{port}} -6 {{host_ip}} {{telnet}}`

- Guess FTP credentials using usernames and passwords lists, specifying the number of threads:

`hydra -e nsr -L {{path/to/usernames.txt}} -P {{path/to/wordlist.txt}} -t {{n_tasks}} {{host_ip}} {{ftp}}`

- Guess MySQL credentials using a username and a passwords list, exiting when a username/password pair is found:

`hydra -e nsr -l {{username}} -P {{path/to/wordlist.txt}} -f {{host_ip}} {{mysql}}`

- Guess RDP credentials using a username and a passwords list, showing each attempt:

`hydra -e nsr -l {{username}} -P {{path/to/wordlist.txt}} -V {{rdp://host_ip}}`

- Guess IMAP credentials on a range of hosts using a list of colon-separated username/password pairs:

`hydra -e nsr -C {{path/to/username_password_pairs.txt}} {{imap://[host_range_cidr]}}`

- Guess POP3 credentials on a list of hosts using usernames and passwords lists, exiting when a username/password pair is found:

`hydra -e nsr -L {{path/to/usernames.txt}} -P {{path/to/wordlist.txt}} -M {{path/to/hosts.txt}} -F {{pop3}}`
