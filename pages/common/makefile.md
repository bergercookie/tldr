# Makefile

> A makefile is a file containing a set of directives used by a make build
> automation tool to generate a target/goal..
> More information: <https://www.gnu.org/software/make/manual/html_node/Introduction.html>

- Create a Makefile function:

```Makefile
define generate_file
    sed 's/{NAME}/$(1)/' greetings.tmpl >$(2).txt
endef
```

- Call a Makefile function:

`$(call generate_file,John Doe,101)`
