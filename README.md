# Within Reach Media to VR180

Within Reach Media to VR180 converts flat images and video into fixed-position
VR180 media on macOS.

## Beta 1

This first public beta is for Apple Silicon Macs running macOS 26 or later.
It supports:

- still-image and flat-video sources;
- deterministic fixed-position VR180 projection and preview;
- 6K standard output and 8K recommended output;
- 50, 59.94, and 60 fps production timelines;
- H.265 output, with VideoToolbox acceleration and a bundled libx265 fallback;
- transparent MOV output for compositing;
- Fast mode for short-turnaround review exports.

## Install

1. Download the DMG from the
   [latest prerelease](https://github.com/ao-huangxr/within-reach-media-to-vr180/releases/tag/v0.1.0-beta.1).
2. Open the DMG and copy **Within Reach Flat Media VR180** to Applications.
3. Launch the app from Applications.

The app is signed with Developer ID, notarized by Apple, and includes its own
FFmpeg runtime. Homebrew, a source checkout, system Python, and user `PATH`
configuration are not required.

## Known limitations

- Beta projects are not guaranteed to remain backward-compatible with later
  beta builds.
- This release is Apple Silicon only and has no Windows package.
- It produces fixed-position VR180 media; it does not perform automatic subject
  tracking, camera-motion reconstruction, or depth-aware scene conversion.
- 8K output is recommended for final headset review but takes substantially
  longer and requires more storage than 6K.
- Hardware H.265 availability and speed depend on the Mac model. The bundled
  libx265 fallback is slower.
- Always keep original source media and independently review important output
  in the target headset and finishing workflow.

## Privacy

Media processing is performed locally. The app does not upload project media.
The optional update check contacts the public GitHub Pages appcast and GitHub
Release download endpoints.

## Feedback

Report reproducible bugs through
[GitHub Issues](https://github.com/ao-huangxr/within-reach-media-to-vr180/issues).
Include the macOS version, Mac model, export format, frame rate, relevant error
text, and the app's copied diagnostics. Do not attach private source media unless
you intend to publish it.

## Licensing

The application and bundled third-party components have separate terms. See
[LICENSE](LICENSE) and [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md). Exact
FFmpeg 8.1.2 and x265 4.2 source archives are attached to the release.
