---
type: guideline
trigger: When extracting location metadata from local JPEG files and third-party EXIF tooling may be unavailable.
owner: visahak
visibility: public
published_at: 2026-04-18T01:51:20Z
---

Use /private/tmp/evolve-codex-demo/tools/exif_gps_extract.py first when a task requires GPS coordinates from a local JPEG in a minimal environment.

## Rationale

It extracts EXIF GPS data directly from the JPEG TIFF structure without exiftool or Pillow, which avoids dependency failures in stripped-down shells.
