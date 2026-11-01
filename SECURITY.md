# Security Policy

Thank you for helping keep **Secure Development** and its users safe.

## Supported versions

This repository has no versioned releases. Only the current `main` branch is
supported; security fixes are applied there.

## Reporting a vulnerability

**Please do not open a public issue for security problems.**

Report privately through GitHub's private vulnerability reporting:

1. Open <https://github.com/vitorparras/Secure-Development/security/advisories/new>.
2. Describe the problem, where it is, how to reproduce it and the impact you
   expect. A proof of concept is welcome but not required.

If you cannot use GitHub, e-mail <contato.vitorparras@gmail.com> with the same
information. Put `[SECURITY] Secure-Development` in the subject.

## What to expect

| Step | Target |
|---|---|
| Acknowledgement of your report | within 3 business days |
| Initial assessment and severity | within 7 days |
| Fix or mitigation for confirmed issues | within 90 days, sooner for critical issues |
| Public disclosure | coordinated with you after the fix is available |

You will be credited in the advisory unless you prefer to stay anonymous.

## Scope

In scope:

- Content in this repository that would lead a reader to an insecure practice
  (for example, an example that is vulnerable by construction without saying so).
- Code, scripts, configuration and GitHub Actions workflows in this repository.
- Supply-chain issues: dependencies, pinned actions, build and release process.

Out of scope:

- Vulnerabilities in third-party tools or services that are only referenced here.
- Issues that require physical access to a maintainer's machine or account.

## Safe harbor

Good-faith research that follows this policy is authorized. We will not pursue
legal action against researchers who avoid privacy violations, data destruction
and service disruption, and who give us reasonable time to fix the issue before
disclosing it.

## How this repository is protected

- `main` only receives changes through pull requests; force pushes and branch
  deletion are blocked.
- Secret scanning with push protection, Dependabot alerts and security updates,
  and private vulnerability reporting are enabled.
- GitHub Actions are restricted to GitHub-owned and verified creators, pinned by
  commit SHA, with read-only default permissions.
- [OpenSSF Scorecard](https://scorecard.dev) runs weekly and publishes results.
