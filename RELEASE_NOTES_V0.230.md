**StereoMate V0.230** lets you set the nearest and farthest depth points yourself, can limit the positive depth while keeping the stereo window intact, saves JPS, PNG, WebP and TIFF files with stereo tags, and plays videos on one or two extra screens. See the [README](https://github.com/crunchy3d/StereoMate#readme) for everything StereoMate does.

### Which file do I need?
- **Windows:** `StereoMate_0.230.0_x64-setup.exe` (installer), or `StereoMate_0.230.0_portable.exe` (no installation). The `.msi` is an alternative installer.
- **Linux:** `StereoMate_0.230.0_amd64.AppImage` (make it executable and start it) or the `.deb` package.
- **Web version (Chrome / Edge):** `StereoMate_web_0.230.0.zip`. Unpack it and open `StereoMate.html`; keep `opencv.js` in the same folder. It has fewer capabilities than the desktop program. You can also [try it online](https://crunchy3d.github.io/StereoMate/).

Windows may show “Windows protected your PC” because the program is not code-signed: click **More info → Run anyway**.

### New since V0.224
- **Depth points:** mark the nearest and / or farthest point yourself when the automatic ones are wrong (e.g. tiles or other repeating patterns). The depth values and the stereo window follow your points; the alignment does not change.
- **Limit positive depth** to a value of your choice (e.g. 3.333 %): too deep scenes are shifted forward, but never so far that an object at the left or right edge breaks the window — or fully, with an automatic floating window if you allow it.
- **Manual points:** if no partner is found, you can place it yourself.
- **File types:** JPS, PNG, WebP and TIFF besides JPG, optionally with stereo tags; TIFF images can be loaded too.
- **Second screen:** two separate screens (one view each), several screens together, and video clips and compositions playing there in step with the main window.
- **Image only (I):** fills the screen exactly; the main window can be mirrored in this mode for mirror stereoscopes.

Questions and problems: please open an [Issue](https://github.com/crunchy3d/StereoMate/issues).
