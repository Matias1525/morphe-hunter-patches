# Morphe Hunter Patches

Experimental YouTube Hunter patch source for Morphe.

## Remote source

After the repository is public, add this in Morphe Manager:

`github.com/Matias1525/morphe-hunter-patches`

Morphe reads `patches-bundle.json` and downloads the latest released `.mpp`.

## Current scope

- Search results only
- Hunter on/off
- Diagnostic logs
- Minimum duration
- Hide Shorts
- Require auto-dub marker

## Update flow

GitHub Actions builds a new `.mpp`, publishes a release, and refreshes `patches-bundle.json`. Morphe can then see the update from the same remote source.

Upstream: `MorpheApp/morphe-patches`
Target upstream tag: `v1.44.0-dev.4`
Hunter version: see `VERSION`.
