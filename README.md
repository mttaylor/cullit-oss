# Cullit

> Cull the noise from your releases. AI-powered release notes that don't suck.

[![npm](https://img.shields.io/npm/v/cullit.svg)](https://www.npmjs.com/package/cullit)
[![CI](https://github.com/mttaylor/cullit-oss/actions/workflows/ci.yml/badge.svg)](https://github.com/mttaylor/cullit-oss/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Sponsor](https://img.shields.io/github/sponsors/mttaylor?label=Sponsor&logo=github)](https://github.com/sponsors/mttaylor)

Cullit turns a noisy git log into clean, customer-facing release notes — using your existing PR descriptions, commit messages, and (optionally) issues from Jira/Linear.

## Quick start

```bash
npx cullit generate --from v1.0.0 --to v1.1.0
```

Or as a GitHub Action:

```yaml
- uses: mttaylor/cullit-oss@v2
  with:
    from: ${{ github.event.before }}
    to: ${{ github.sha }}
```

## Packages

| Package | Description |
|---------|-------------|
| [`cullit`](packages/cli) | CLI — `npx cullit generate` |
| [`@cullit/core`](packages/core) | Core library: collectors, generators, formatters |
| [`@cullit/config`](packages/config) | Configuration loader |
| [`@cullit/pro`](packages/pro) | Pro features (license-key gated) |
| [`@cullit/licensed`](packages/licensed) | License verification helpers |

## Features

- **Git log collection** — pulls commits and PRs between any two refs
- **AI summarization** — OpenAI / Anthropic / Ollama / none
- **Issue enrichment** — Jira and Linear integrations
- **Multiple formats** — Markdown, JSON, plain text
- **GitHub Action** — drop-in CI workflow

## Support the project

If Cullit saves you time, consider [sponsoring on GitHub](https://github.com/sponsors/mttaylor) or starring the repo. Every bit helps keep it maintained.

## License

MIT — see [LICENSE](LICENSE).

## Hosted version

Looking for a hosted dashboard, billing, and team features? Visit [cullit.io](https://cullit.io).
