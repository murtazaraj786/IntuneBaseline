# memory.md — IntuneBaseline (THIS REPO IS BEING RETIRED)

Last updated: 2026-07-11.

## Status: superseded, pending deletion

This repo is a fork of `SkipToTheEndpoint/OpenIntuneBaseline`. Earlier in this
project it got an automated JSON validation test suite (800 assertions across
all 114 policy files, encoding-aware UTF-16/UTF-8 handling, CI added — see
`tests/` and `.github/workflows/ci.yml` if this repo is still around when you
read this).

**Since then**, the project owner decided this repo should become a fully
standalone (non-fork) repo, and be expanded from Intune-only into a
multi-product security baselines repo also covering Microsoft Defender for
Endpoint, Defender for Office 365, Defender for Cloud Apps, and Microsoft
Purview. That work is happening in a **new repo: `SecurityBaselines`**
(`github.com/murtazaraj786/SecurityBaselines`), not here.

The plan (confirmed with the project owner):
1. Content from this repo (`WINDOWS/`, `MACOS/`, `WINDOWS365/`, `BYOD/`,
   `tests/`, etc.) moves into `SecurityBaselines/INTUNE/` unchanged, with full
   git history preserved via a local staging clone + restructure.
2. New top-level folders added to `SecurityBaselines/` for the other 4
   products, each with its own README, tests, and CI.
3. **This repo (`IntuneBaseline`) gets deleted** once the content is safely
   pushed to `SecurityBaselines`.

If you're reading this and `IntuneBaseline` still exists, either the
`SecurityBaselines` repo hasn't been created yet (blocked on the GitHub App
integration lacking repo-creation permission — the project owner needs to
create it manually at github.com/new), or the deletion step just hasn't
happened yet. Check `github.com/murtazaraj786/SecurityBaselines` first before
doing any new work in this repo — see that repo's `memory.md` for full
current state.
