# Contributing

This repository maintains the Magrathean UK profile and project index. Corrections to public descriptions, links, and documentation belong here. Product bugs and feature requests belong in the relevant product's own support channel.

## Repository map

| Path | Purpose |
| --- | --- |
| `README.md` | Public company profile and project links |
| `assets/icons/` | Product artwork |
| `profile-3d-contrib/` | Generated contribution graphs |
| `github-metrics.svg` | Existing metrics artwork |
| `.github/workflows/profile-3d.yml` | Contribution-graph generation workflow |
| `LICENSE`, `license.md`, `TRADEMARKS.md` | Legal notice and licensing guidance |
| `SECURITY.md` | Private reporting and existing safe-harbour terms |
| `AGENTS.md`, `CLAUDE.md` | Editing guidance for coding assistants |

## Propose a correction

Use the [issue tracker](https://github.com/magrathean-uk/magrathean-uk/issues) for a broken link or factual correction. Include the affected section and a public source for the replacement. Read [LICENSE](LICENSE) before preparing changes; the repository is proprietary and this guide does not grant additional rights.

Do not include private repository names, internal endpoints, account information, credentials, or unreleased product details. Send sensitive reports through [SECURITY.md](SECURITY.md).

## Check a documentation change

1. Check product descriptions against their public sites or repositories. Preserve distinctions between source code, public product documentation, and design-stage projects.
2. Open changed external links without relying on authentication. Check each relative document or image path, including case.
3. Preview Markdown with GitHub-flavoured Markdown support. Check headings, lists, tables, and the contribution graph.
4. Run `git diff --check` from the repository root and review the diff for unrelated changes. This checks tracked working-tree edits; review newly added files too.
5. Preserve legal text and attribution. Explain any unresolved factual or link check in the review.

No dependency installation, application build, or local server is needed. The existing `.claude/launch.json` starts a separate sibling website and is not a profile preview.

## Generated artwork

The existing workflow runs on a daily schedule, manual dispatch, and changes to its own workflow file on `main`. It uses `yoshi389111/github-profile-3d-contrib@latest` with a repository token and writes generated output back to the repository. A README-only change does not trigger its push path filter. Keep workflow and generated-artwork changes out of unrelated prose corrections.

For development across the linked software projects, consider [Clean Development](https://github.com/magrathean-uk/clean-development) to organise supported caches and build output.
