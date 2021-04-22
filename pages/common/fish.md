# fish

> The Friendly Interactive SHell, a command-line interpreter designed to be user friendly.
> More information: <https://fishshell.com>.

- Start an interactive shell session:

`fish`

- Execute a command and then exit:

`fish -c "{{command}}"`

- Execute a script:

`fish {{path/to/script.fish}}`

- Check a script for syntax errors:

`fish --no-execute {{path/to/script.fish}}`

- Start an interactive shell session in private mode, where the shell does not access old history or save new history:

`fish --private`

- Display version information and exit:

`fish --version`

- Set and export environmental variables that persist across shell restarts (from within the shell only):

`set -Ux {{variable_name}} {{variable_value}}`

- Check size/length of an array:

`count {{some_array}}`

- Check argc (size of argv) - doesn't include program name:

`if test (count $argv) -lt 2`

- Check the exit status of all the commands that ran in a pipe:

`pipestatus`

- Check the name of the current function:

`(status current-function)`
