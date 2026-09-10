# linely

Learning Rust by rewriting coreutils, one tool at a time

Built for my own use; public in case it helps someone.

## Examples

```bash
./target/release/linely src/*.rs
cat README.md | ./target/release/linely
```

## Getting started

```bash
cargo build --release
```

## Features

- Zero dependencies outside std
- Reads stdin or multiple files
- Counts lines, words and bytes like wc
- Parallel over files with std threads

## Project structure

```text
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── development.md
│   └── faq.md
├── examples/
│   └── quickstart.md
├── src/
│   └── main.rs
├── .gitignore
├── CHANGELOG.md
├── Cargo.toml
├── LICENSE
└── SECURITY.md
```

## Development

```bash
cargo build
cargo clippy -- -D warnings
```

## Notes

- mostly stable, edge cases remain

## License

MIT licensed, see LICENSE.
