# Security Policy

## Supported Versions

| Version | Supported |
|---------|-----------|
| Latest  | ✅ Yes    |
| Older   | ❌ No     |

We recommend always using the latest published version of TypeSharp.

## Reporting a Vulnerability

**Please do not report security vulnerabilities via public GitHub issues.**

If you discover a security vulnerability, report it responsibly by opening a [GitHub Security Advisory](https://github.com/typesharp-cli/typesharp/security/advisories/new) in the repository.

Include:
- A description of the vulnerability
- Steps to reproduce
- Potential impact
- Any suggested fixes (optional)

We will acknowledge your report within **72 hours** and aim to resolve confirmed vulnerabilities promptly.

## Scope

This policy applies to:
- `typesharp-cli/typesharp` — the core CLI tool
- `typesharp-cli/TypeSharp.Attributes` — the attributes NuGet package

TypeSharp is a code generation tool and does not handle authentication, user data, or network requests at runtime. The primary security concern is around safe parsing of C# source files and safe file output.
