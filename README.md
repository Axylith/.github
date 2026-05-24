# .github

This repository holds organization-level configuration for [Axylith](https://github.com/Axylith).

It is NOT the editor source. The editor lives at [Axylith/axle](https://github.com/Axylith/axle).

## What's in here

| Path | Purpose |
|------|---------|
| `profile/README.md` | The org landing page shown at [github.com/Axylith](https://github.com/Axylith) |
| `README.md` | This file — explains the repo to anyone who navigates here directly |
| `assets/` | SVG assets used by the org profile (banner, thesis, projects cards) |
| `dependabot.yml` | Dependabot config applied to this repo |
| `ISSUE_TEMPLATE/` | Default issue templates inherited by all repos in the org that don't define their own |
| `PULL_REQUEST_TEMPLATE.md` | Default PR template inherited by all repos in the org |
| `SECURITY.md` | Org-wide security policy (vulnerability reporting) |
| `CODE_OF_CONDUCT.md` | Org-wide code of conduct |
| `CONTRIBUTING.md` | Default contributing guide |

## How GitHub uses this repo

A repository named exactly `.github` inside an organization has special behavior:

- **`profile/README.md`** auto-renders as the organization's landing page
- **`ISSUE_TEMPLATE/*`**, **`PULL_REQUEST_TEMPLATE.md`**, **`SECURITY.md`**, **`CODE_OF_CONDUCT.md`**, **`CONTRIBUTING.md`** are used as defaults for any repo in the org that doesn't define its own

This means editing files here updates defaults across every Axylith repository at once. Be careful with changes.

## Editing

1. Open a PR against `main`
2. CI runs (currently just SVG validation if we add it)
3. Merge after review

Changes to `profile/` take effect immediately on the org page after merge. Changes to issue templates affect new issues going forward; existing issues are unaffected.

## Image references

All SVGs in `profile/README.md` use absolute `raw.githubusercontent.com` URLs rather than relative paths. This is because `profile/README.md` is rendered out-of-tree by GitHub's org-page system, and relative paths break in that context. Don't switch them to relative paths — they will appear broken.

## Related repositories

- **[Axylith/axle](https://github.com/Axylith/axle)** — the editor source (AGPL v3 + commercial dual-license)
- **[Axylith/bots](https://github.com/Axylith/bots)** — maintainer automation toolkit (planned, Apache 2.0)
- **[Axylith/physics](https://github.com/Axylith/physics)** — computational physics engine (planned, Apache 2.0)
- **[Axylith/.github-private](https://github.com/Axylith/.github-private)** — internal onboarding & docs (private, org members only)

---

<sub>Built in Calgary, Canada.</sub>
