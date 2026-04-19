# AuroraKai VPM Listing

A [VRChat Creator Companion](https://vcc.docs.vrchat.com/) (VCC) package listing published by Kai.

**Listing URL:** `https://aurorakai.github.io/vpm/index.json`
**Landing page:** <https://aurorakai.github.io/vpm/>

## Add this listing to VCC

One-click (opens VCC): [**Add to VCC**](https://aurorakai.github.io/vpm/) — use the "Add to VCC" button on the landing page.

Or manually:

1. Open VRChat Creator Companion → **Settings** → **Packages** → **Add Repository**
2. Paste `https://aurorakai.github.io/vpm/index.json`
3. Click **Add**, then **I Understand**

Once added, packages from this listing appear in VCC's package picker for any VRChat project.

## Packages

_No packages are published in this listing yet. Check back soon._

When packages are added, they'll appear on the [landing page](https://aurorakai.github.io/vpm/) and in VCC.

## How this repo works

This repository is a VPM listing — a JSON index of VRChat packages that live in their own separate repositories. The `index.json` and landing page are rebuilt automatically by GitHub Actions whenever [`source.json`](source.json) changes.

Key files:

- [`source.json`](source.json) — the listing configuration (identity, and the lists of package repos to index).
- [`.github/workflows/build-listing.yml`](.github/workflows/build-listing.yml) — the workflow that builds `index.json` and publishes to GitHub Pages.
- [`Website/`](Website/) — Scriban templates for the landing page; values are filled in from `source.json` at build time.

The build uses VRChat's [`package-list-action`](https://github.com/vrchat-community/package-list-action) to fetch each listed package's releases from GitHub, merge them into a VPM-compatible `index.json`, and deploy to GitHub Pages.

## Issues & feedback

Found a problem with the listing, or want to suggest a package? Open an [issue](https://github.com/aurorakai/vpm/issues).

Packages indexed by this listing are covered by their own licenses — see each package's repository.
