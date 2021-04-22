# iptables

> Program that allows configuration of tables, chains and rules provided by the Linux kernel firewall.
> More information: <https://www.netfilter.org/projects/iptables/>.

- List all rules in iptables-save style:

`iptables -S`

- View chains, rules, and packet/byte counters of the `filter` table:

`sudo iptables -vnL`

- Add a LOG rule - view logs in `journalctl` or `/var/log/kern.log`:

`sudo iptables -t nat -A POSTROUTING -j LOG --log-prefix "NAT3:" --log-level 7`

- Set chain policy rule:

`sudo iptables -P {{chain}} {{rule}}`

- Append rule to chain policy for IP:

`sudo iptables -A {{chain}} -s {{ip}} -j {{rule}}`

- Append rule to chain policy for IP considering protocol and port:

`sudo iptables -A {{chain}} -s {{ip}} -p {{protocol}} --dport {{port}} -j {{rule}}`

- Show iptables configuration with line numbers:

`sudo iptables iptables -nL -v --line-numbers -t nat`

- Delete chain rule:

`sudo iptables -D {{chain}} {{rule_line_number}}`

- Save iptables configuration of a given table to a file:

`sudo iptables-save -t {{tablename}} > {{path/to/iptables_file}}`

- Restore iptables configuration from a file:

`sudo iptables-restore < {{path/to/iptables_file}}`
