# KRATE pre-release testing checklist

Edit this file on the `develop` branch before each **pre-release** build.
It is published as `TESTING.md` on GitHub Releases (`vX.Y.Z-alpha.N` tags only).

Report issues with the tag and your platform key (e.g. `debian13-amd64`).

## Platform update

- [ ] `zen pull --check` reports the expected target version
- [ ] `zen pull` installs without apt errors
- [ ] HarmonyUI loads after update (hard refresh)

## HarmonyUI

- [ ] Login and dashboard widgets
- [ ] App Store: install / update / remove smoke test
- [ ] Settings pages open without 500 errors

## Console

- [ ] `zen software list` and one app status check
- [ ] `zen pull --check` on beta channel matches this release

## Known risks / focus for this build

- _Describe what changed and what testers should exercise._

## Out of scope

- Production data migration — use a lab VM only.
