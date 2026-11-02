# Secure Development

[![Code: AGPL-3.0](https://img.shields.io/badge/Code-AGPL--3.0-blue.svg)](LICENSE)
[![Content: CC BY-SA 4.0](https://img.shields.io/badge/Content-CC%20BY--SA%204.0-blue.svg)](LICENSE-CONTENT)
[![OpenSSF Scorecard](https://api.scorecard.dev/projects/github.com/vitorparras/Secure-Development/badge)](https://scorecard.dev/viewer/?uri=github.com/vitorparras/Secure-Development)
[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
[![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

Guidelines, tools and checklists for building software securely: secure coding,
vulnerability mitigation, security testing and supply-chain hygiene.

> **Status:** starting. The repository structure and conventions are defined
> below; material is added over time. Contributions are welcome from day one.

## Table of contents

- [Goal](#goal)
- [Planned structure](#planned-structure)
- [Conventions](#conventions)
- [This repository practices what it documents](#this-repository-practices-what-it-documents)
- [References](#references)
- [Contributing](#contributing)
- [Security](#security)
- [Code of conduct](#code-of-conduct)
- [License](#license)

## Goal

A practical companion for developers who want to ship secure software without
becoming full-time security specialists: what to do, why, and how to verify it.
Everything here should be actionable and backed by a reference.

## Planned structure

```text
Secure-Development/
├── guidelines/
│   ├── secure-coding-practices.md     # input validation, output encoding, authn/authz, crypto, errors, logging
│   ├── secrets-management.md
│   └── dependency-and-supply-chain.md
├── vulnerabilities/
│   ├── owasp-top-10.md                # each category: what it is, example, how to prevent, how to test
│   └── common-weaknesses.md           # CWE-based catalog with mitigations
├── tools/
│   ├── static-analysis/               # CodeQL, Semgrep, SonarCloud configurations
│   ├── dynamic-analysis/              # OWASP ZAP configurations and scripts
│   └── dependency-scanning/           # Dependabot, OSV-Scanner, Trivy
├── testing/
│   ├── web-application-test-plan.md
│   └── threat-modeling.md             # STRIDE walkthrough and templates
├── checklists/
│   ├── pull-request-security-review.md
│   └── release-security-checklist.md
└── README.md
```

## Conventions

- **Every recommendation cites a source** (OWASP, NIST, CWE, vendor
  documentation) and says which risk it addresses.
- **Examples show the insecure and the secure version** side by side, clearly
  labeled. Insecure samples must never be runnable against real systems.
- **Tool configurations are tested** against a sample project and state the
  tool version they were written for.
- **No real secrets, hostnames or personal data** anywhere, including in
  examples of "what not to do".

## This repository practices what it documents

- `main` is protected: changes land only through pull requests with passing
  checks; force pushes and deletion are blocked.
- Secret scanning with push protection, Dependabot alerts and security updates,
  and private vulnerability reporting are enabled.
- GitHub Actions are limited to GitHub-owned and verified creators, pinned to
  commit SHAs, with read-only default permissions.
- [OpenSSF Scorecard](https://scorecard.dev/viewer/?uri=github.com/vitorparras/Secure-Development)
  runs weekly and publishes its results.

## References

- [OWASP Top 10](https://owasp.org/Top10/)
- [OWASP Application Security Verification Standard (ASVS)](https://owasp.org/www-project-application-security-verification-standard/)
- [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org/)
- [OWASP Software Assurance Maturity Model (SAMM)](https://owaspsamm.org/)
- [CWE Top 25](https://cwe.mitre.org/top25/)
- [NIST Secure Software Development Framework (SSDF)](https://csrc.nist.gov/projects/ssdf)
- [OpenSSF Scorecard](https://scorecard.dev) and [SLSA](https://slsa.dev)

## Contributing

New guidelines, tool configurations and corrections are welcome. Please read
[CONTRIBUTING.md](CONTRIBUTING.md) first and open a
[suggestion](https://github.com/vitorparras/Secure-Development/issues/new?template=content_suggestion.yml)
before writing a large document.

## Security

Found content that would lead a reader to an insecure practice, or a problem in
this repository's configuration? Follow [SECURITY.md](SECURITY.md) and report
it privately.

## Code of conduct

This project follows the [Contributor Covenant](CODE_OF_CONDUCT.md). By
participating you agree to uphold it.

## License

This repository uses two licenses:

- **Code** (programs, scripts, configuration files and code samples):
  [GNU Affero General Public License v3.0](LICENSE) (AGPL-3.0).
- **Content** (documents, explanations, images and other non-code material):
  [Creative Commons Attribution-ShareAlike 4.0 International](LICENSE-CONTENT)
  (CC BY-SA 4.0).

Both require attribution, and both require that modified versions you
distribute, sell or run as a network service remain under the same license.
Copyright © Vitor Hugo Parras.
