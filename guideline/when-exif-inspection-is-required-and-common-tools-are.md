---
type: guideline
trigger: When reading image metadata in sandboxed or minimal workspaces with limited installed packages.
owner: visahak
visibility: public
published_at: 2026-04-18T01:51:20Z
---

When EXIF inspection is required and common tools are missing, prefer a dependency-free local parser over trying multiple absent utilities.

## Rationale

This avoids wasted retries like exiftool not installed and PIL not installed, and gets directly to the working path in constrained environments.
