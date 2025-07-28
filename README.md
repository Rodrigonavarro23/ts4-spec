
# TS4 – Technical Specs for AI

**TS4** is a lightweight YAML format designed to capture technical decisions, implementation rules, and key code references. Its primary goal is to provide clear, structured context easily understood by both developers and artificial intelligence agents.

![TS4 Logo](logo.png)

## Why TS4?

- 📚 **AI-Ready Context**: Ideal for use with embeddings, RAG, and LangChain agents.
- 🔍 **Technical Clarity**: Clear, traceable, and maintainable rules.
- ⚡ **Developer Friendly**: Easy-to-maintain YAML files.
- 🌐 **Open Standard**: Intended as an open specification.

## Example

```yaml
ts4: "1.0"
id: "TS4-004"
title: "System Input Validations"
summary: "Validate data at controllers; internal services assume data validity."
rules:
  - "Avoid repeating validations in internal services"
  - "Provide clear errors with 4xx HTTP status codes"
code_refs:
  - "handlers/user.go"
  - "pkg/validation/*.go"
```

## Getting Started

1. Create a `/ts4` folder in your repository.
2. Add `.ts4` files for each technical decision or rule set.
3. Optionally index with ChromaDB or another embedding engine for AI queries.

## License

Public domain under [The Unlicense](LICENSE).
