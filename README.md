This repository is intended to curate a list of Rust crates for writing debuggers and other related tools. We also have an IRC channel for discussion on irc.mozilla.org, #rust-debugger-tools.

# List of useful crates

## Mature

* [gimli](https://github.com/gimli-rs/gimli) - DWARF parser
* [goblin](https://github.com/m4b/goblin) - Parser for binary formats (ELF/Mach-O/PE)
* [object](https://github.com/gimli-rs/object) - A cross-platform abstraction built atop goblin to unify handling of various object file formats
* [addr2line](https://github.com/gimli-rs/addr2line) - A simple interface built atop gimli to look up source file/line/function information given an address in a binary
* [capstone](https://github.com/capstone-rust/capstone-rs) - Rust interface to the [capstone](http://capstone-engine.org/) multi-architecture disassembly framework (x86/x86-64/arm/aarch64 and more)

## Working

* [pdb](https://github.com/willglynn/pdb) - Parser for Microsoft PDB format debugging symbols


## Experimental

* [moria](https://github.com/gimli-rs/moria) - Locate detached debug symbols
* [minidump](https://github.com/luser/rust-minidump) - Parser for Microsoft minidump crash report files
* [disasm](https://github.com/luser/rust-disasm) - A tool for producing source-interleaved disassembly built using object+moria+addr2line+capstone

## Work in progress

* [gdb-remote-protocol](https://github.com/luser/rust-gdb-remote-protocol) - Implementation of the [GDB remote protocol](https://sourceware.org/gdb/onlinedocs/gdb/Remote-Protocol.html)
* [pdb-download](https://github.com/jrmuizel/pdb-downloader) - Fetch PDB symbols from a symbol server