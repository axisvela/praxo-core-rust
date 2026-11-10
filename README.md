# PRAXO-CORE for Rust

Dedicated repository for the Rust implementation of PRAXO-CORE: an embeddable,
MIT-licensed agent execution kernel with policy controls, human-in-the-loop
approval, checkpoints, events, and tool calling.

- Package: `praxo-core` on crates.io
- Documentation: https://axisvela.github.io/praxo-core/languages/rust/
- Canonical source: https://github.com/axisvela/praxo-core/tree/main/language/rust
- Release index: https://axisvela.github.io/praxo-core/languages/registry-status/

This repository is a discovery mirror of the canonical Rust source. The monorepo
remains the source of truth and the release workflow source. Shared conformance
vectors are included under `spec/`.

## Install

```sh
cargo add praxo-core@0.3.0
```

## Verify

From `language/rust`:

```sh
cargo test
cargo run --quiet --bin conformance
python api-snapshot.py --check
```

PRAXO-CORE is not a hosted model, workflow engine, identity provider, or safety
controller. Do not infer exactly-once execution, complete sandbox isolation,
production security certification, live-provider behavior, or physical safety
from this package.

MIT licensed.
