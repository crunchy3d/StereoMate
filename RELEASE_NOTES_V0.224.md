**StereoMate V0.224** measures depth of images that were already aligned in other programs, gives images and videos their own output size (with black bars or filled frames), supports mirror stereoscopes on the second screen, and fills the stereo show from the list automatically. See the [README](https://github.com/crunchy3d/StereoMate#readme) for everything StereoMate does.

### Which file do I need?
- **Windows:** `StereoMate_0.224.0_x64-setup.exe` (installer), or `StereoMate_0.224.0_portable.exe` (no installation). The `.msi` is an alternative installer.
- **Linux:** `StereoMate_0.224.0_amd64.AppImage` (make it executable and start it) or the `.deb` package.
- **Web version (Chrome / Edge):** `StereoMate_web_0.224.0.zip`. Unpack it and open `StereoMate.html`; keep `opencv.js` in the same folder. It has fewer capabilities than the desktop program. You can also [try it online](https://crunchy3d.github.io/StereoMate/).

Windows may show “Windows protected your PC” because the program is not code-signed: click **More info → Run anyway**.

### New since V0.221
- **Only measure depth** for images already aligned elsewhere (e.g. StereoPhoto Maker): depth values, extreme points and the remaining vertical error, without changing the image.
- **New layout:** *Stereo alignment* (with Fine-tuning at its bottom), a new card **Crop and window**, and *Export* before *Create stereo show*.
- **Separate output sizes for images and videos**, with *Fit*: whole image with black bars, fill and trim the edges, or no bars. Time-lapses now take their size from Export.
- **Second screen for mirror stereoscopes:** each half can be mirrored or rotated. Swap views there is now the key **X**.
- **Image only** on the whole screen (key **I**, back with I or Esc) and new shortcuts **B** (Edit crop), **C** (Compose), **V** (Create stereo show), **M** / **Shift+M** (Auto-match). The help lists all shortcuts (⌨ Shortcuts).
- **Sound** in the video clip preview.
- **Create stereo show** adds the images and clips of the list automatically, aligned as they are; you choose what happens with images that have no depth values.

Questions and problems: please open an [Issue](https://github.com/crunchy3d/StereoMate/issues).
