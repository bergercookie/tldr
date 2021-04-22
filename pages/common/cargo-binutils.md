# cargo-binutils

> Cargo subcommands to invoke the LLVM tools shipped with the Rust toolchain.

- List all symbols in an executable sorted by size (smallest first):

`cargo nm --release -- -print-size -size-sort`


- Transform the cargo output (ELF) into binary format:

`cargo objcopy --release -- -O binary {{app.bin`}}


- Dissassemble a binary:

`cargo objdump --release -- --disassemble --no-show-raw-insn`

- Dump the symbols of a section in an executable:

`cargo objdump --bin app -- -s --section .vector_table`

- Get the size of a target application:

`cargo size --target {{thumbv7m-none-eabi}} --bin {{app}}`

- Strip all symbols:

`cargo-strip --release -- -strip-all -O {{smaller-hello}}`
