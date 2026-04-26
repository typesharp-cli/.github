# TypeSharp CLI 🔷

> **Automatically generate TypeScript from C# — keep your frontend and backend types in perfect sync.**

TypeSharp is a developer-first CLI tool built for teams working with **ASP.NET Core** backends and **TypeScript** frontends (Vue, Nuxt, React, Angular). Stop duplicating your models. Let TypeSharp do it.

---

## ✨ What We Build

| Repository | Description |
|---|---|
| [`typesharp`](https://github.com/typesharp-cli/typesharp) | The core CLI — scan C# models, output TypeScript interfaces |
| [`TypeSharp.Attributes`](https://github.com/typesharp-cli/TypeSharp.Attributes) | C# attributes for fine-grained control over type generation |

---

## ⚡ Quick Example

```csharp
// C# — your source of truth
public class ProductDto {
    public int Id { get; set; }
    public string Name { get; set; }
    public decimal? Price { get; set; }
    public ProductCategory Category { get; set; }
}
```

```bash
typesharp generate --input ./Models --output ./frontend/types
```

```typescript
// Auto-generated TypeScript
export interface ProductDto {
  id: number;
  name: string;
  price?: number;
  category: ProductCategory;
}
```

---

## 🚀 Features

- ✅ Nullable type support (`T?` → `T | undefined`)
- ✅ Enum generation
- ✅ Inheritance & base class resolution
- ✅ Array and collection types
- ✅ Custom naming conventions (camelCase, PascalCase)
- ✅ Fine-grained control via `[TypeSharp]` attributes
- ✅ Perfect for ASP.NET Core + Vue/Nuxt/React projects

---

## 📦 Installation

```bash
dotnet tool install --global TypeSharp.Cli
```

---

## 🤝 Contributing

We welcome contributions! Check out our [Contributing Guide](https://github.com/typesharp-cli/.github/blob/main/CONTRIBUTING.md) to get started.

---

## 📍 Based in South Africa 🇿🇦
