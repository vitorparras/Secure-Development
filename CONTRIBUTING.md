# Contributing to Secure Development

Thank you for your interest. This is an open, community-friendly study
repository: corrections, new material and better explanations are all welcome.

By participating you agree to follow the [Code of Conduct](CODE_OF_CONDUCT.md).
Security problems go through [SECURITY.md](SECURITY.md), never through a public
issue.

## Ways to contribute

- **Fix a mistake**: open a [correction issue][correction] or a pull request.
- **Propose new material**: open a [suggestion issue][suggestion] first so we can
  agree on scope before you write it.
- **Improve clarity**: better wording, examples, diagrams or references.
- **Translate**: when a document exists in only one language, a translation to
  English or Brazilian Portuguese is welcome. Keep both versions in sync.

[correction]: https://github.com/vitorparras/Secure-Development/issues/new?template=content_error.yml
[suggestion]: https://github.com/vitorparras/Secure-Development/issues/new?template=content_suggestion.yml

## Content guidelines

- **Be correct and cite sources.** Prefer official documentation, specifications
  and peer-reviewed material. Add a link when you state something non-obvious.
- **Explain, do not only show.** Every example should say what it demonstrates
  and why it matters.
- **Keep the existing structure.** Follow the folder layout and naming described
  in the README. One topic per file or folder.
- **Write your own text.** Do not paste copyrighted content. Short quotes with
  attribution are fine.
- **Code must run.** Include the language or tool version it was tested with.
  Keep examples minimal and free of secrets, credentials or personal data.
- **No large binaries.** Images should be small (prefer SVG or compressed PNG).
  Datasets and compiled artifacts do not belong in Git; link to them instead.

## Pull request workflow

1. Fork the repository and create a branch from `main`:
   `git switch -c <type>/<short-description>` (for example `content/linq-basics`).
2. Make focused changes. One topic per pull request keeps review fast.
3. Use clear commit messages in English. [Conventional Commits][cc] are
   appreciated: `docs: add question about async streams`.
4. Open the pull request against `main` and fill in the template. Link the issue
   it resolves.
5. A maintainer will review it. Please respond to comments; stale PRs may be
   closed after 30 days of inactivity.

`main` is protected: changes only land through pull requests, and all automated
checks must pass.

[cc]: https://www.conventionalcommits.org/

## Licensing of contributions

Code contributions are licensed under the [AGPL-3.0](LICENSE) and content
contributions (text, images, documents) under [CC BY-SA 4.0](LICENSE-CONTENT),
the same licenses as the repository. By opening a pull request you confirm that
you have the right to license your contribution under those terms.

## Questions

Use [Discussions](https://github.com/vitorparras/Secure-Development/discussions) for
questions and ideas that are not yet concrete issues.
