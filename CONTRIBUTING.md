# Contributing

Thanks for your interest in contributing to this repo! Contributions — fixes, enhancements, examples, and documentation — are welcome. Please follow the guidelines below to help keep the project healthy and reviewable.

## Reporting issues

- Search existing issues before opening a new one.
- Provide a clear title and description, steps to reproduce, expected vs actual behavior, and the relevant environment information (`rustc --version`, `cargo --version`, OS).
- Include a minimal reproduction when possible.

## Submitting pull requests

1. Fork the repository and create a topic branch with a descriptive name (for example `fix/readme-typo` or `feat/day-02-examples`).
2. Keep changes focused and small — one logical change per PR.
3. Run tests and checks locally:

```sh
cargo test
cargo fmt -- --check
cargo clippy -- -D warnings
```

4. Update or add documentation where appropriate (README, day README files, or examples).
5. Write a clear PR description that explains the motivation and any user-visible changes. Link the issue if applicable.

## Code style

- Use `rustfmt` for formatting. The repository follows default `rustfmt` settings.
- Fix lint warnings reported by `clippy` when practical; keep the codebase clean.

## Tests and CI

- Add tests for bug fixes and new features when feasible.
- CI runs on PRs to run the test and lint suite. Ensure your branch passes the checks before requesting review.

## Examples and Solutions

- Place new example code under the appropriate `day-*/examples/` folder.
- Add solution references under `day-*/solutions/` when providing full solutions.

## License

By contributing you agree that your contributions will be licensed under the repository's license (see `LICENSE`).

## Code of Conduct

Be respectful and constructive. If you'd like a formal Code of Conduct added, please open an issue.

## Questions

Open an issue or contact the repository owner via GitHub for questions or help.

Thank you — happy hacking! 🦀
