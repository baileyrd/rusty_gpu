# rusty_gpu — archived, moved to Rusty Mill

**This repository is archived.** `rusty_gpu` now lives in the
[Rusty Mill monorepo](https://github.com/Rusty-Mill/rusty_mill) as
[`crates/rusty_gpu`](https://github.com/Rusty-Mill/rusty_mill/tree/main/crates/rusty_gpu),
with full commit history preserved via `git subtree`. Please file issues
and pull requests against the new location — this repo is read-only.

If you depend on this crate via a `git` dependency, repoint it at
`https://github.com/Rusty-Mill/rusty_mill.git` (the crate name is
unchanged, so Cargo's git dependency resolution still finds it).

---

*The README below is preserved as it was at the time of the merge, for
historical reference.*

# rusty_gpu

A `#![no_std]` + `alloc` sovereign CPU software framebuffer presenter and SIMD
vector rasterizer for the **Rusty Mill** ecosystem — draws into an in-memory
pixel buffer and presents it to an OS window without going through a GPU API.

## Status
Experimental — early scaffold (`Framebuffer`, `Color`, a minimal `Pipeline`
with rectangle fill). Owned by [@baileyrd](https://github.com/baileyrd).

## Getting started
```bash
git clone https://github.com/baileyrd/rusty_gpu
cd rusty_gpu
cargo build
```

## Architecture
See [ARCHITECTURE.md](./ARCHITECTURE.md) for boundaries, key decisions, and data flow.

## Development
```bash
cargo test
cargo clippy -- -D warnings
cargo fmt --check
```

## Contributing
See [CONTRIBUTING.md](./CONTRIBUTING.md).

## Security
See [SECURITY.md](./SECURITY.md) to report a vulnerability.

## License
MIT OR Apache-2.0
