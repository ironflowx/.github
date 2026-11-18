# Contributing

Thanks for helping. This file applies to every ironflowx repository that has no CONTRIBUTING.md of its own. Where a repository has its own guide (or a CLAUDE.md / docs folder with rules), that guide wins.

## Before you start

- For anything larger than a small fix, open an issue first so we can agree on the approach.
- Read the repository's README and docs. Some projects record design decisions as ADRs in `docs/decisions/`. A change that contradicts one needs a new ADR.
- Security problems go through [SECURITY.md](SECURITY.md), not public issues.

## Making a change

1. Fork the repository and create a branch from the default branch.
2. Keep each pull request to one change.
3. A bug fix starts with a test that fails without the fix.
4. Run the same checks as CI before you push. For the Rust projects:

   ```sh
   cargo fmt --all --check
   cargo clippy --workspace --all-targets -- -D warnings
   cargo test --workspace
   ```

5. Write commit messages that say why the change was made, not only what changed.

## Licensing

By submitting a contribution, you agree it is licensed under the license of the repository you contribute to (see its LICENSE file).
