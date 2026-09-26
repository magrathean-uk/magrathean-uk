# Repository guide

This repository holds the Magrathean UK GitHub profile and public project index. It contains Markdown, artwork, and a contribution-graph workflow, with no application package or local build command.

Complete authorized work and the necessary safe local steps through the relevant checks. Make routine decisions without repeated permission requests. Use bounded delegation for independent work when it helps, with clear ownership.

## Editing boundaries

- Keep `README.md` focused on the public company and project index. Verify that each listed repository and product link is publicly reachable before adding it.
- Describe product status from its own current public documentation. Do not infer source availability, readiness, or licence terms from a repository name.
- Preserve exact legal grants, ownership notices, attribution, and the safe-harbour terms in `SECURITY.md`. See [license.md](license.md) and [TRADEMARKS.md](TRADEMARKS.md).
- Keep private projects, credentials, internal infrastructure, and unreleased work out of public content.
- Treat `profile-3d-contrib/` and `github-metrics.svg` as generated assets. Do not regenerate them for a prose edit. Keep workflow changes relevant to the task.
- `.claude/launch.json` targets a sibling website. It is not a preview command for this repository.

## Validation

Run `git diff --check` for working-tree edits. Preview changed Markdown, check relative links and images, and open changed public links without relying on a signed-in account. Record any unavailable link instead of claiming it was verified.

The repository defines no dependency-install command, build command, or application test suite. Complete the relevant document checks and report their limits. See [Contributing](CONTRIBUTING.md) for the repository map and review checklist.
