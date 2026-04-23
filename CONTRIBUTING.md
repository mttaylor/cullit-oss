# Contributing to Cullit

Thanks for your interest in contributing! Cullit is MIT-licensed, and we welcome bug reports, feature requests, and pull requests.

## Development setup

```bash
git clone https://github.com/mttaylor/cullit-oss.git
cd cullit-oss
pnpm install
pnpm build
pnpm test
```

Requires Node.js 22+ and pnpm 10+.

## Project layout

This is a pnpm workspace with five packages:

- `packages/core` — collectors, generators, formatters
- `packages/cli` — `cullit` CLI binary
- `packages/config` — config loader
- `packages/pro` — Pro features
- `packages/licensed` — license verification

## Pull requests

1. Fork and create a feature branch
2. Add tests for new behavior
3. Run `pnpm lint && pnpm test && pnpm build` before pushing
4. Open a PR against `main` with a clear description

## Code of Conduct

See [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md).

## License

By contributing, you agree your contributions will be licensed under the MIT License.
