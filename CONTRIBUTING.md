# Contributing

Welcome. Default contribution guidance for Axylith repositories.

Individual repos may have their own `CONTRIBUTING` that overrides parts of this. Check the repo first.

## Before you start

1. **Search existing issues.** Your idea or bug may already be tracked.
2. **Open an issue first** for non-trivial changes. A short discussion saves both of us from doing work that won't merge.
3. **Read the repo's `README` and any architecture docs.** Understanding what's already there shapes what fits.

## Pull requests

- **One concern per PR.** Don't bundle a refactor with a new feature; split them.
- **Write a clear description.** What changed, why, how to verify. Link the issue if there is one.
- **Match the existing style.** If the repo uses `clang-format` or `ruff`, run them. If naming conventions exist, follow them.
- **Add tests** for new behavior, regression cases for bugs.
- **Disclose AI assistance.** If Claude, Copilot, or similar tools wrote material portions of the code, say so in the PR.
- **Keep commits coherent.** `git rebase -i` before opening if your commit history is messy.

## Style and tooling

Each repo defines its own. Some general expectations across Axylith:

- **No unjustified warnings.** Fix or suppress with a comment explaining why.
- **No dead code.** If you removed a feature, remove its tests and references too.
- **No unrelated changes.** A PR titled "fix typo" should not also reformat 50 files.
- **Sanitizers must pass** in repos with sanitizer CI. AddressSanitizer / UBSan failures aren't optional.

## Code of Conduct

All contributors are expected to follow the [Code of Conduct](CODE_OF_CONDUCT.md).

## License

Submitting a PR means you agree that your contribution will be licensed under the repository's existing license (typically AGPL v3 for `axle`, Apache 2.0 for others). If the repository uses a CLA, you'll be asked to sign it before your first PR is merged.

## How review works

- One maintainer review approval is required for merge
- CI must pass (build matrix, tests, sanitizers, lint)
- Conventional commit messages preferred but not required
- Squash or rebase merge depending on the repo's setting (default: squash)

## What helps your PR get merged faster

- A clear title that summarizes the change
- A description that explains the *why*, not just the *what*
- A small, focused change rather than a sprawling one
- Tests covering the new behavior
- Responses to review comments within a reasonable timeframe (a week, ideally)

## Questions

- Open an issue with the `question` label
- For sensitive topics, email the maintainer of the affected repo directly
