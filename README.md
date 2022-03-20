# rust-zero2prod

Inner development loop:

```bash
cargo install cargo-watch
cargo watch -x check -x test -x run
```

Coverage:

```bash
cargo install cargotarpaulin
cargo tarpaulin --ignore-tests
```

Linting:

```bash
rustup component add clippy
cargo clippy -- -D warnings
```

Formatting:

```bash
rustup component add rustfmt
cargo fmt --  --check
```

Security Vulnerabilities

```bash
cargo install cargo-audit
cargo audit
```