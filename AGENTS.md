# Repository guide

This repository holds the Magrathean UK GitHub profile and public project index. It contains Markdown, artwork, and a contribution-graph workflow, with no application package or local build command.

Complete authorized work and the necessary safe local steps through the relevant checks. Make routine decisions without repeated permission requests. Use bounded delegation for independent work when it helps, with clear ownership.

## Editing boundaries

- Keep `README.md` focused on the public company and project index. Verify that each listed repository and product link is publicly reachable before adding it.
- Describe product status from its own current public documentation. Do not infer source availability, readiness, or licence terms from a repository name.
- Preserve exact legal grants, ownership notices and attribution in `LICENSE` and `.github/SECURITY.md`. The account-wide [legal notice](https://github.com/magrathean-uk/.github/blob/main/LEGAL.md) covers names and trade marks; do not duplicate it here.
- Legal files (`LICENSE`, `NOTICE`, `docs/legal/`, contributor terms, copyright and
  attribution strings) are owner-controlled: change them only on the owner's explicit
  instruction.
- Keep private projects, credentials, internal infrastructure, and unreleased work out of public content.
- Treat `profile-3d-contrib/` as a generated asset. Do not regenerate it for a prose edit. Keep workflow changes relevant to the task.
- Use an icon from `assets/icons/` in the product grid only when one exists for that product; otherwise leave the icon cell blank rather than adding new artwork.
- `.claude/launch.json` targets a sibling website. It is not a preview command for this repository.

## Validation

Run `git diff --check` for working-tree edits. Preview changed Markdown, check relative links and images, and open changed public links without relying on a signed-in account. Record any unavailable link instead of claiming it was verified.

The repository defines no dependency-install command, build command, or application test suite. Complete the relevant document checks and report their limits. See [Contributing](.github/CONTRIBUTING.md) for the repository map and review checklist.

<!-- clean-development-policy:v1 (canonical text: ~/dev/source/dev-bootstrap/snippets/clean-development-policy.md) -->
## Clean development (mandatory)

This project follows [Clean Development](https://github.com/magrathean-uk/clean-development) and the machine rule that nothing creates tool state under `~` (only the allow-listed agent homes).

- The shell environment comes from `~/.zshenv`, which loads `~/dev/env.zsh`. It routes every tool home and cache (`CARGO_HOME`, `RUSTUP_HOME`, `XDG_*`, `BUNDLE_USER_HOME`, `npm_config_cache`, `XCODE_DERIVED_DATA_PATH`, ...) and switches telemetry off. Never unset, override or bypass those variables. If a script needs a scrubbed environment, re-export them with `source ~/dev/env.zsh`.
- Run builds, tests, installs and anything else that writes caches or build output through Clean Development: `clean-development run --session session-only -- <command>`. Follow its docs and keep its receipts.
- Do not add installers or scripts that default into `~` (`~/.cargo`, `~/.rustup`, `~/.cache`, `~/.npm`, `~/.swiftpm`, `~/.gradle`, ...) and do not hardcode `$HOME` paths for caches; use the routed variables.
- Before finishing, run `dev-env-check` (must pass) and `dev-audit` (no new entries in `~`). If your work caused a violation, fix the cause in the repo and say so.
