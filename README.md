# Morphe Hunter Patches

Experimental YouTube Hunter patch layer for Morphe.

## Goal

Keep YouTube's own search/recommendation system and filter the rendered results locally inside Morphe.

Initial experimental scope:
- YouTube search results only
- Hunter enable/disable switch
- Diagnostic logs
- Minimum duration filter
- Hide Shorts
- Require Morphe's auto-dub radar marker

## Build model

This repository does **not** duplicate the full Morphe source tree.

GitHub Actions:
1. clones the exact upstream Morphe Patches tag,
2. applies `hunter-v0.1.patch`,
3. builds the Morphe patch bundle,
4. uploads the generated `.mpp` as an artifact.

Upstream base: `MorpheApp/morphe-patches`
Target base tag: `v1.44.0-dev.4`

This keeps the Hunter changes small and makes rebasing onto future Morphe versions much easier.
