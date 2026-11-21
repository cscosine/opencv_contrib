# Changelog of the cscosine fork of opencv_contrib

## v5.1.0-cpu.2 (and v5.1.0-cuda.1, to tag once csopencvcuda has built it)

- No change here: the tag follows the opencv fork's `v5.1.0-cpu.2` (an MLAS fix), so both forks keep the same tags.

## v5.1.0-cpu.1 (never released: the Linux clang builds of opencv failed)

- On upstream `5.1.0`, with the opencv fork's layout: `main`, `cpu`, `cuda`, the same tags.
- The `vec_traits.hpp` Win32 fix is dropped: upstream has it.

## Before (history)

`v5.0.0-cpu`, `v5.0.0-cuda`: upstream 5.0.0 plus the `vec_traits.hpp` Win32 fix (branches `dev-*` / `main-*`).
`v5.0.0-original`: upstream 5.0.0 (branch `main-original`).
