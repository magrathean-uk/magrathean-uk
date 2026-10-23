# Repository context

This repository holds the Magrathean UK GitHub profile and public project index. It contains Markdown, artwork and a contribution-graph workflow, with no application package or local build command.

## Repository map

- `README.md`: public company and product index.
- `assets/icons/`: product artwork used by the grid.
- `profile-3d-contrib/`: generated contribution-graph asset.
- `.claude/launch.json`: a sibling website's launch target.
- [.github/CONTRIBUTING.md](.github/CONTRIBUTING.md): repository map and document review references.
- `LICENSE` and `.github/SECURITY.md`: legal and security information.
- [Account legal notice](https://github.com/magrathean-uk/.github/blob/main/LEGAL.md): names and trade marks.

## Document checks

`git diff --check` checks patch whitespace. Markdown previews, relative-link checks, image previews and signed-out public-link checks cover different aspects of the public profile. There is no dependency-install command, application build or application test suite in this repository.

## URL migration context

[NEXT-RELEASE-URLS.md](NEXT-RELEASE-URLS.md) describes the release URL migration: product sites use `https://magrathean.uk/solutions/<slug>/` and support addresses use `contact+<slug>@magrathean.uk`.

## Development environment

The machine's `~/dev/machine/env.zsh` provides routed storage variables. `$TMPDIR` identifies session scratch, `$CLEAN_DEV_BUILDS` identifies throwaway build output, and cache variables identify dependency caches. `.clean-development.json` records repository build and dependency directories.
