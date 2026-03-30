# {{SUPPLEMENT_TITLE}}

> **Status:** {{STATUS}}
> **Domain:** IHE Devices (DEV)
> **Revision:** {{REVISION}}

## About This Document

{{DESCRIPTION}}

## Quick Start

### Editing

The supplement source files are in `src/` as AsciiDoc (`.adoc`) files.

- `src/main.adoc` — the master document (includes all other files)
- `src/volume-1.adoc` — Volume 1: Integration Profiles
- `src/volume-2.adoc` — Volume 2: Transactions
- `src/volume-3.adoc` — Volume 3: Content Modules (if applicable)
- `src/metadata.adoc` — supplement metadata (title, status, revision)

### Local Preview

If you have Asciidoctor installed:

```bash
make html    # Render HTML
make pdf     # Render PDF
make all     # Both
make clean   # Remove build output
```

Or use Docker:

```bash
make docker-html
make docker-pdf
```

### Publishing

Push to `main` and the GitHub Actions workflow will automatically:
1. Render the AsciiDoc to HTML and PDF
2. Deploy the output to GitHub Pages

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

---

*This repo was created from [DEV.supplement-template](https://github.com/IHE/DEV.supplement-template).*
