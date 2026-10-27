---
name: magpie-tip-chrome-cycle
description: >-
  Use before every Magpie shell-demo consume, tip bump, or Vercel ship—run the
  why-change / why-delete / chrome regression loop so nest width stays top-tabs
  gold and WEB_SIDE_AT never returns.
---
# Magpie tip chrome cycle

Run **before** coding a consume and again **before** `git push` / Vercel for `/workspace/magpie-shell-demo`.

## Gold (do not “fix”)
- **`SIDE_AT = 1024` only.** Below that = **top tabs** (Win/Mac + nest 752/616). That is Magpie, not a bug.
- Web card **752×652** (v0.1.91) aligns nest responsive — keep it; do not force side-nav into mid widths.
- **Never** reintroduce `WEB_SIDE_AT` (v0.1.98 mistake; removed in v0.1.99).

## Hard rules
- Nest slice only. No silent shell/layout/nav/breakpoint refactors.
- Out-of-slice shell touch needs WHY in `docs/TIP-CHANGELOG.md` + what is preserved.
- `npm run chrome-guard` must pass before tip.

## Loop
1. Baseline tip + commit; confirm no `WEB_SIDE_AT`.
2. Intent: shot range only; list expected files.
3. Out-of-slice check on `App.tsx` / `shell-patch.css` / breakpoints — stop or justify.
4. Implement nest only.
5. `npm run chrome-guard`.
6. Visual: ~752 top tabs; ≥1024 side-nav + graphite `.on`; phoneWeb top tabs.
7. Changelog + ship.

## Related
- `docs/TIP-CYCLE.md`, `docs/TIP-CHANGELOG.md`, `npm run chrome-guard`
- CIS `/workspace/magpie-shell-cis-2026-10-15.md`
