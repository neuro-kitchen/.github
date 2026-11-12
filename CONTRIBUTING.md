# Contributing to neuro-kitchen

Thanks for wanting to help! Contributions from researchers and developers are both welcome.

## Ways to help

- **Report a bug:** open an issue using the bug report template
- **Suggest a feature:** open an issue using the feature request template
- **Improve docs:** typo fixes and clearer explanations are always welcome
- **Write code:** pick an issue labeled `good first issue` or `help wanted`

## Making a change

1. **Fork** the repository and create a branch from the **version branch** the next release is
   built on (`version/v0.0.x`, `versions/v0.0.x` in dsp-kitchen; the newest one), or from `main`
   if the project has none.
2. **Make your change**, keeping each pull request focused on one thing, and each commit on one
   concern.
3. **Add tests** if you change behavior, and make sure existing tests pass.
4. **Update docs** if you change how something is used, and add a line to `CHANGELOG.md` under
   *Unreleased*.
5. **Open a pull request into that version branch** and fill in the template.

All changes go through a pull request and review. Direct pushes to `main` are blocked.

## Releases

A version branch collects the work of one release. When it is ready, a release pull request
into `main` sets the version and moves the changelog's *Unreleased* section under it. After the
merge, the merge commit is tagged `vX.Y.Z`; the release workflow checks the tag against the
version, builds, publishes (crates.io and PyPI through trusted publishing, after a maintainer
approves) and makes the GitHub release from the changelog.

## Guidelines

- **Never commit research data, credentials, or API keys.** Use small synthetic data for tests.
- Follow the existing code style of the project you're working in.
- Write clear commit messages that say what changed and why.

## License

By contributing, you agree that your contributions are licensed under the
[Apache License 2.0](LICENSE), the same license as the project.

## Code of conduct

Please follow our [Code of Conduct](CODE_OF_CONDUCT.md) in all project spaces.
