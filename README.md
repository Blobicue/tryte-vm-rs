# tryte-vm-rs

A Rust port of **tryte-vm**, a balanced-ternary computer: core arithmetic, a
25-instruction machine, an assembler, and an emulator written in its own
assembly.

> **Status: scaffold.** No part of the machine has been ported yet.

## The machine

| | |
|---|---|
| Trit | −1, 0, +1 |
| Tryte | 6 trits — 729 values, **−364 … +364** |
| Memory | 729 cells, addressed **−364 … +364**; address 0 is the *centre* |
| Registers | `A` accumulator, `C` gate/table control, `PC` |
| Instruction | two cells: opcode, operand |
| Instructions | 25 |

## Building

Needs a stable Rust toolchain (see [rustup](https://rustup.rs)).

```bash
cargo build   # library crate
cargo test    # there are no tests yet
```
