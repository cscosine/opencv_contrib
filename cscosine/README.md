# opencv_contrib: the cscosine fork

OpenCV's extra modules, built together with the [opencv fork](https://github.com/cscosine/opencv) by
[csopencvcpu](https://github.com/cscosine/csopencvcpu) (CPU) and [csopencvcuda](https://github.com/cscosine/csopencvcuda)
(CUDA). This folder is ours; the rest of the repository is upstream.

It follows the opencv fork's layout exactly: the same upstream release, the same branches, the same tags. The
layout, the versions and the sync procedure are described once, in
[opencv's `cscosine/README.md`](https://github.com/cscosine/opencv/blob/main/cscosine/README.md).

| | |
|---|---|
| Upstream | <https://github.com/opencv/opencv_contrib> (remote `upstream`; its tags are fetched, its branches are not copied) |
| Base | upstream tag `5.1.0` |
| License | upstream's (`LICENSE`, Apache-2.0) |

## Branches

- `main`: upstream `5.1.0` plus this folder (`git log 5.1.0..main`).
- `cpu`, `cuda`: the same as `main`. The variant is chosen by opencv's setup, so contrib needs no commit of its own;
  the branches exist so that both forks are tagged the same way (`v<opencv>-cpu.<n>` on `cpu`, `v<opencv>-cuda.<n>`
  on `cuda`).

## Our changes

None besides this folder. The Win32 fix we carried on 5.0.0 (`vec_traits.hpp`, `long long` for CUDA's 64-bit
vector types) is in upstream 5.1.0.

Older tags stay, because released builds point to them: `v5.0.0-cpu`, `v5.0.0-cuda`, `v5.0.0-original` and
`legacy-main-*` (the branches before this layout).
