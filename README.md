# No-Crop Border Tool

A tiny, single-file browser tool that adds borders to your photos so they fit
Instagram's dimensions **without cropping**. Pick photos, choose a format, save.

- **Free & ad-free**, no watermark, no sign-up.
- **Private** — everything runs in your browser. Photos are never uploaded to any server.
- **Works offline** once the page has loaded, and works great on a phone.

## Use it

Open `index.html` in any browser. On your phone, add it to the home screen for
one-tap access.

1. Tap **Choose photos** (pick one or several from your gallery).
2. Pick an Instagram **format**:
   - **Best fit** — automatically adds the least border possible while staying
     within Instagram's allowed range (1.91:1 landscape → 4:5 portrait).
   - **Square** 1:1, **Portrait** 4:5, **Landscape** 1.91:1, **Story** 9:16.
3. Choose a **border color** — white, black, a custom color, or a blurred
   version of your own photo as the background.
4. Optionally add **extra margin** or **rounded corners**.
5. Tap **Save** (or **Save all** for a batch).

Your whole image is always shown — the border fills the rest so nothing is cut off.

## Saving on a phone

After tapping Save, long-press the resulting image and choose “Save to Photos”,
or use the browser's share sheet. Output is a high-quality JPEG at 1080px on the
short edge (Instagram's native size).

## Tech

Plain HTML + CSS + JavaScript using the Canvas API. No dependencies, no build
step. EXIF orientation is respected so phone photos aren't rotated. The single
`index.html` is the whole app.
