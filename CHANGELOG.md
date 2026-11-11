# Changelog

## V0.224 (November 2026)

Changes since V0.221 (V0.222 and V0.223 were not published separately):

- **Already aligned images:** *Images are already aligned — only measure depth* (top of *Stereo alignment*) finds the matching points and measures the depth values, extreme points and the remaining vertical error, but changes nothing (no correction, no stereo window, no crop). The status compares the error with what a new alignment would give and marks clearly worse images with ⚠.
- **New layout:** *Auto-alignment* is now **Stereo alignment** with *Fine-tuning* at its bottom; the new card **Crop and window** holds the crop and the floating window. *Export* now comes before *Create stereo show*.
- **Size per view for images and for videos** (Export), each with **Fit** for a fixed size: whole image with black bars (the file is exactly W × H), fill and trim the edges, or whole image without bars. For videos *Original* and *Scale* refer to the original video frame; time-lapses take their size from here (the size fields of the render window are gone). Very large video sizes are pointed out.
- **Second screen:** the left / top and right / bottom part can each be mirrored (horizontally, vertically) or rotated (90° left / right, 180°) — for mirror stereoscopes, e.g. two monitors joined into one screen. Swap views in the second-screen window is now **X**.
- **Image only:** key **I** shows only the image on the whole screen; **I** or **Esc** brings the normal window back.
- **New shortcuts:** **B** Edit crop on / off, **C** Compose, **V** Create stereo show, **M** / **Shift+M** Auto-match current / all. The help has a **⌨ Shortcuts** button with all keys.
- **Sound in the video clip preview** (🔊 next to Loop; MP4 / MOV).
- **Create stereo show takes the list:** each time it is opened, the images and clips of the main list that are not in the show yet are added — aligned images as they are now in the main window (they follow later changes), rendered clips from their rendered file. For images without alignment or depth values you choose: measure their depth, add without depth (not counted in the show's depth values) or add only the aligned ones. **Add images of the list** adds missing ones again.

## V0.221 (November 2026)

Changes since V0.218 (V0.219 and V0.220 were not published separately):

- **Rotation of the views:** 90° clockwise, 180° or 90° counter-clockwise for the left and the right view, for all images (Input) or per image / clip (Fine-tuning) — for cameras mounted on their side or upside down and images without EXIF orientation. Works for images, time-lapses and video clips (rotated on the graphics card); the **rotation tag** of phone videos (left + right files, mono videos) is applied automatically.
- **Apply to all images per section:** Fine-tuning, crop, floating window and manual brightness / colour values can each be copied to all other images; every such button (and *Apply current values to all images*) asks first and can be undone.
- **Changed or renamed files:** when a session's files are missing, **Choose folder with changed files…** finds images corrected in another program by the same name, a detected name pattern (e.g. “_edit”, “-1”), an own rule or the EXIF capture time, shown in a table to confirm; **Choose replacements…** and **Replace file…** (one image or several images from a folder) work the same way. The images keep all their settings (scaled to a new size of the same shape).
- **Shortcuts after editing a field:** a click on the image or the preview area leaves the edit field, so the keyboard shortcuts work at once.
- **Crop editing:** the hint “Editing the crop…” is shown above the image instead of on it; fixed: clicking *✂ Edit crop on the image* could shift the whole window up.

## V0.218 (November 2026)

- **Frame rates:** rendered video clips, compositions and the stereo show use the frame rate of their videos by default (e.g. 25 fps); images-only shows and time-lapses use 30 fps. Every video output has a **Frames / s** field with **↺** (back to the default). A clip can be rendered at another rate (frames are repeated or skipped, the sound stays in sync).
- **Frame-rate warnings:** when clips with different frame rates are combined, or the output rate differs from the source, an orange note explains it, and before rendering with uneven rates (e.g. 25 → 30) StereoMate asks: use the source rate, render anyway, or cancel. Exact multiples (25 ↔ 50) only get a note; 29.97 counts as 30.
- **New views in the main window:** row interleaved and column interleaved (passive 3D monitors) and checkerboard (DLP 3D), drawn at screen pixels, with **Swap L / R**; the pattern follows when the window is moved.
- **Size per view when saving** (Export): original, fit inside 1920 × 1080 or 3840 × 2160, fit inside any W × H, long side, width or scale (%), with **Never enlarge**; the size refers to one view and the resulting file size is shown.

## V0.217 (November 2026): first public version

StereoMate has been developed privately since early 2026; this is the first version published on GitHub.
Main features of this version (see the README for the full list):

- Automatic alignment of stereo pairs (rotation, size, vertical shift, vertical and horizontal perspective, stereo window), manual points, fine-tuning, barrel distortion correction.
- Depth values with comfort warnings and extreme points; folders for too deep results.
- Crop (X / Y relative to the automatic crop of the aligned image), floating window, brightness and colour matching.
- All common input and output formats (side-by-side, over-under, interleaved, MPO, JPS, left + right files, anaglyph).
- Compose: several images in one picture, with frames and depth-safe layouts; **new: video clips and time-lapses in a composition, rendered as a video** (start time per clip, hold last frame or loop, sound from a chosen clip).
- Video clips: key frames, rendering on the graphics card to MP4 with 3D tag; left + right files synchronised by sound or motion (also uncompressed PCM sound, e.g. Sony XAVC S); stereo from a mono video taken while moving sideways.
- **New: time-lapses as one entry** (Open time-lapse…, Group as time-lapse…), aligned once or with key frames, rendered at any frame rate.
- Create stereo show: slide show with motion, transitions, text slides, music and narration.
- Second screen for monitors, projectors and 3D TVs.
- Clip bar with a fixed Play / Pause button; **Enter** = Play / Pause.
- Help in English, German, French, Dutch and Slovenian.
- Web version shows a note about the features that need the desktop program.
