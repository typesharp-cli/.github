# Contributing to TypeSharp

Thank you for your interest in contributing to TypeSharp! 🎉  
Whether it's a bug fix, new feature, or documentation improvement — all contributions are welcome.

---

## 📋 Before You Start

- Check existing [issues](https://github.com/typesharp-cli/typesharp/issues) to avoid duplicates.
- For large changes, open an issue first to discuss the approach.
- All contributions must target the `main` branch unless otherwise specified.

---

## 🛠️ Development Setup

### Prerequisites

- [.NET SDK 8+](https://dotnet.microsoft.com/download)
- Git

### Clone & Build

```bash
git clone https://github.com/typesharp-cli/typesharp.git
cd typesharp
dotnet restore
dotnet build
```

### Run Tests

```bash
dotnet test
```

---

## 🔄 Pull Request Process

1. Fork the repository.
2. Create a feature branch: `git checkout -b feat/your-feature-name`
3. Make your changes with clear, focused commits.
4. Ensure all tests pass: `dotnet test`
5. Update relevant documentation if needed.
6. Open a Pull Request against `main` and fill in the PR template.

### Commit Message Format

Use conventional commits:

```
feat: add support for record types
fix: resolve nullable enum generation bug
docs: update README with new CLI flags
chore: bump dependencies
```

---

## 🧪 Adding Tests

All new features and bug fixes should include tests.  
Tests live in the `tests/` directory and use xUnit.

---

## 📁 Project Structure

```
typesharp/
├── src/
│   ├── TypeSharp.Cli/         # CLI entry point
│   ├── TypeSharp.Core/        # Parsing & generation logic
│   └── TypeSharp.Attributes/  # C# attributes (separate repo)
└── tests/
    └── TypeSharp.Tests/       # Unit + integration tests
```

---

## 🤝 Code of Conduct

By participating, you agree to follow our [Code of Conduct](./CODE_OF_CONDUCT.md).
