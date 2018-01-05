This repository is intended to curate a list of Rust crates for writing debuggers and other related tools. We also have an IRC channel for discussion on irc.mozilla.org, #rust-debugger-tools.

# List of useful crates

## Mature

* [gimli](https://github.com/gimli-rs/gimli) [![](https://docs.rs/gimli/badge.svg)](https://docs.rs/gimli/) - DWARF parser
* [goblin](https://github.com/m4b/goblin)  [![](https://docs.rs/goblin/badge.svg)](https://docs.rs/goblin/) - Parser for binary formats (ELF/Mach-O/PE)
* [object](https://github.com/gimli-rs/object) [![](https://docs.rs/object/badge.svg)](https://docs.rs/object/) - A cross-platform abstraction built atop goblin to unify handling of various object file formats
* [addr2line](https://github.com/gimli-rs/addr2line) [![](https://docs.rs/addr2line/badge.svg)](https://docs.rs/addr2line/) - A simple interface built atop gimli to look up source file/line/function information given an address in a binary
* [capstone](https://github.com/capstone-rust/capstone-rs) [![](https://docs.rs/capstone/badge.svg)](https://docs.rs/capstone/) - Rust interface to the [capstone](http://capstone-engine.org/) multi-architecture disassembly framework (x86/x86-64/arm/aarch64 and more)
* [cpp_demangle](https://github.com/gimli-rs/cpp_demangle)  A crate for demangling C++ symbols.

## Working

* [pdb](https://github.com/willglynn/pdb) [![](https://docs.rs/pdb/badge.svg)](https://docs.rs/pdb/) - Parser for Microsoft PDB format debugging symbols
* [spawn-ptrace](https://github.com/luser/spawn-ptrace) [![](https://docs.rs/spawn-ptrace/badge.svg)](https://docs.rs/spawn-ptrace/) - Spawn a child process with ptrace enabled
* [spawn-task-port](https://github.com/luser/rust-spawn-task-port/) [![](https://docs.rs/spawn-task-port/badge.svg)](https://docs.rs/spawn-task-port/) - Spawn a child process on macOS and get a hold of its Mach task port
* [read-process-memory](https://github.com/luser/read-process-memory) [![](https://docs.rs/read-process-memory/badge.svg)](https://docs.rs/read-process-memory/) - Read memory from another process
* [elfkit](https://github.com/aep/elfkit) [![](https://docs.rs/elfkit/badge.svg)](https://docs.rs/elfkit/) - ELF manipulation for writing tools like binutils

## Experimental

* [moria](https://github.com/gimli-rs/moria) - Locate detached debug symbols
* [minidump](https://github.com/luser/rust-minidump) - Parser for Microsoft minidump crash report files
* [disasm](https://github.com/luser/rust-disasm) - A tool for producing source-interleaved disassembly built using object+moria+addr2line+capstone
* [tracetree](https://github.com/luser/tracetree) [![](https://docs.rs/tracetree/badge.svg)](https://docs.rs/tracetree/) - Trace a process and all of its children on Linux

## Work in progress

* [gdb-remote-protocol](https://github.com/luser/rust-gdb-remote-protocol) - Implementation of the [GDB remote protocol](https://sourceware.org/gdb/onlinedocs/gdb/Remote-Protocol.html)
* [pdb-download](https://github.com/jrmuizel/pdb-downloader) - Fetch PDB symbols from a symbol server
