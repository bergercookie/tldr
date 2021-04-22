# nasm

> The Netwide Assembler, a portable 80x86 assembler.
> More information: <https://nasm.us>.

- Assemble `source.asm` into a binary file `source`, in the (default) raw binary format:

`nasm {{source.asm}}`

- Assemble `source.asm` into a binary file `output_file`, in the ELF64 format:

`nasm -f elf64 {{source.asm}} -o {{output_file}}`

- Assemble `source.asm` into a binary file `output_file`, with debugging symbols:

`nasm -f {{format}} {{source.asm}} -F dwarf -g -o {{output_file}}`

- List valid output formats (along with basic nasm help):

`nasm -hf`

- Assemble and generate an assembly listing file:

`nasm -l {{list_file}} {{source.asm}}`

- Add a directory (must be written with trailing slash) to the include file search path before assembling:

`nasm -i {{path/to/include_dir/}} {{source.asm}}`
