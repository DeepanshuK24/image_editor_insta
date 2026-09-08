# No-Crop Border Tool

A tiny, single-file browser tool that adds borders to your photos so they fit
Instagram's dimensions **without cropping**. Pick photos, choose a format, save.

- **Free & ad-free**, no watermark, no sign-up.
- **Private** — everything runs in your browser. Photos are never uploaded to any server.
- **Works offline** once the page has loaded, and works great on a phone.

## Use it

Open `index.html` in any browser. On your phone, add it to the home screen for
one-tap access.

## Host it on your phone (GitHub Pages)

Give the tool its own permanent web address so it opens straight in Chrome — no
login, no app viewer. One-time setup:

1. On GitHub, open this repo → **Settings** → **Pages** (left sidebar).
2. Under **Build and deployment → Source**, choose **Deploy from a branch**.
3. Set **Branch** to `claude/instagram-border-tool-aeb1rg` and folder to
   **/ (root)**, then **Save**.
4. Wait ~1 minute. Your tool will be live at:
   **https://deepanshuk24.github.io/image_editor_insta/**
5. Open that URL in Chrome on your phone and add it to your home screen.

> Tip: opening the tool inside the Claude app's built-in viewer can block the
> photo picker (Android's in-app web view doesn't always support file uploads).
> A real browser like Chrome — including the GitHub Pages URL above — avoids this.

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
