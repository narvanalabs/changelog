# Narvana Changelog

[![Astro](https://img.shields.io/badge/Astro-5.0-BC52EE?style=flat&logo=astro&logoColor=white)](https://astro.build/)
[![Bun](https://img.shields.io/badge/Bun-Runtime-f9f1e1?style=flat&logo=bun&logoColor=black)](https://bun.sh/)
[![License](https://img.shields.io/badge/License-Apache_2.0-blue?style=flat)](https://github.com/narvanalabs/control-plane/blob/main/LICENSE)

Release notes and changelog for Narvana - the modern PaaS platform.

## Development

```bash
# Install dependencies
bun install

# Start development server
bun run dev

# Build for production
bun run build
```

## Adding Releases

Release entries are automatically generated when a new version is tagged in the control-plane repository. The GitHub Actions workflow:

1. Creates a release entry markdown file in `src/content/releases/`
2. Generates an SVG banner for the release
3. Commits and pushes the changes

### Manual Release Entry

To manually add a release, create a markdown file in `src/content/releases/` with the following frontmatter:

```markdown
---
title: "Narvana v1.0.0"
date: "2026-01-07"
versionNumber: "1.0.0"
description: "Brief description of the release"
image:
  src: "../../assets/release-1_0_0.svg"
  alt: "Narvana v1.0.0 Release"
---

## What's New

Your release content here...
```

### Custom Banners

To use a custom banner instead of the auto-generated one, place your SVG file at:
`src/assets/custom/release-{version_underscore}.svg`

For example, for version 1.0.0: `src/assets/custom/release-1_0_0.svg`

## License

Apache License 2.0 - see the control-plane repository for details.
