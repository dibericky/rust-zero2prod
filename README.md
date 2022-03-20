# rust-zero2prod

## Set Up

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

Security Vulnerabilities:

```bash
cargo install cargo-audit
cargo audit
```

Adding Dependencies:

```bash
cargo install cargo-edit
```

Debug macros

```bash
cargo install cargo-expand
cargo +nightly expand
```


## Users stories

- As a blog visitor, I want to subscribe to the newsletter, so that I can receive email updates when new content is published on the blog;
- As the blog author, I want to send an email to all my subscribers, so that I can notify them when new content is publishes;
- As a subscriber, I want to be able to unsubscribe from the newsletter, so that I can stop receiving email updates from the blog;