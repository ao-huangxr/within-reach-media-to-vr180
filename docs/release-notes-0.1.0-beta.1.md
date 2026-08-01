# Within Reach Media to VR180 0.1.0 Beta 1

The first public macOS Apple Silicon beta converts flat images and video into
fixed-position VR180 media.

## Included

- Project creation and reopening.
- Flat image and video import.
- Deterministic VR180 preview.
- 6K standard and 8K recommended output.
- 50, 59.94, and 60 fps timelines.
- H.265 export with Fast mode and bundled libx265 fallback.
- Transparent MOV export for compositing workflows.
- Signed Sparkle 2 update checks.
- Bundled FFmpeg 8.1.2 runtime; Homebrew and system Python are not required.

## Beta limitations

- Apple Silicon and macOS 26 or later only.
- No Windows package.
- Projects are not guaranteed to remain backward-compatible with later betas.
- Final media should be reviewed in the target headset and finishing workflow.
- 8K production output requires substantially more time and storage than 6K.

## Integrity

Verify downloads against `SHA256SUMS.txt`. The DMG and app are signed with
Developer ID and notarized by Apple. Exact FFmpeg and x265 source archives are
provided with this release.
