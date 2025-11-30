# FlakeCache Crate Index

Private Cargo registry index for FlakeCache Rust crates.

## Usage

Add to `~/.cargo/config.toml` or `.cargo/config.toml`:

```toml
[registries.flakecache]
index = "sparse+https://raw.githubusercontent.com/FlakeCache/crate-index/main/"

[net]
git-fetch-with-cli = true
```

Then in `Cargo.toml`:

```toml
[dependencies]
chunker = { version = "0.1.0-beta7", registry = "flakecache" }
```

## Crates

- **chunker** - High-performance content-defined chunking for Nix NARs (Rustler NIF + standalone library)
