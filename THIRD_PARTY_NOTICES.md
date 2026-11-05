# Third-party components

StereoMate (MIT licence, Copyright (c) 2026 Damir Vrančić) includes or uses the following components.
Their licences apply to those components.

| Component | Use in StereoMate | Licence |
|---|---|---|
| [OpenCV.js](https://opencv.org) 4.10.0 | feature detection and matching, image warping | Apache License 2.0 — full text in `dist/opencv-LICENSE.txt` inside the project archive and the web version |
| [mp4-muxer](https://github.com/Vanilagy/mp4-muxer) 5.2.2 | writing MP4 files (bundled in the program, slightly extended for the stereo 3D tag) | MIT License, Copyright (c) 2023 Vanilagy — notice kept in the program source |
| [Tauri](https://tauri.app) 2 and its Rust / JavaScript dependencies | desktop program (window, file access) | MIT or Apache License 2.0 |
| [ffmpeg](https://ffmpeg.org) | optional, **not included**: used by the desktop program only if the user installs it | LGPL / GPL (user's own installation) |

The Microsoft Edge WebView2 runtime (Windows) and WebKitGTK (Linux) are system components, not part of StereoMate.
