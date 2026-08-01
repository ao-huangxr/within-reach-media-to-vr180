# Third-Party Notices

Within Reach Flat Media VR180 includes or uses the following third-party
software. Each component remains subject to its own license.

## FFmpeg 8.1.2

- Project: <https://ffmpeg.org/>
- License for this build: GNU GPL version 2 or later
- Reason: the bundled command-line runtime includes the x265 encoder
- Corresponding source release asset:
  `ffmpeg-8.1.2-within-reach-source.tar.xz`
- Source SHA-256:
  `464beb5e7bf0c311e68b45ae2f04e9cc2af88851abb4082231742a74d97b524c`

The app invokes the bundled FFmpeg runtime as a separate command-line process.
The FFmpeg build configuration and license text are also embedded in the app.

## x265 4.2

- Project: <https://bitbucket.org/multicoreware/x265_git/>
- License: GNU GPL version 2 or later, or a commercial license from the project
- Corresponding source release asset: `x265-4.2-within-reach-source.tar.gz`
- Source SHA-256:
  `40b1ea0453e0309f0eba934e0ddf533f8f6295966679e8894e8f1c1c8d5e1210`

## Sparkle 2.9.2

- Project: <https://sparkle-project.org/>
- License: MIT

Sparkle supplies the signed update framework, updater app, XPC services, and
official appcast/signing tools.

## Qt for Python / PySide6

- Project: <https://doc.qt.io/qtforpython-6/>
- Version in this release: 6.11.1
- Licensing: LGPLv3/GPLv3 or commercial, depending on the component and use

## Python

- Project: <https://www.python.org/>
- Version in this release: 3.12.2
- License: Python Software Foundation License

Additional notices and license files are embedded under
`Contents/Resources/licenses` in the application bundle.
