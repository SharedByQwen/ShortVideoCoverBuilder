# ShortVideoCoverBuilder

**CoverLab** is a lightweight, browser-based Instagram cover designer. It runs entirely on the client: no backend, account, build step, or image upload is required.

## Features

- Persian and English headline text with playful display fonts
- Live preview with layered text outlines (inner and customizable outer border)
- Editable fill, border, subtitle, background, and gradient colors
- Ready-made outline color palette
- Optional local background image and adjustable dark overlay
- Instagram portrait (4:5), square (1:1), and story (9:16) canvases
- PNG export at 1080px wide
- Settings autosave in the current browser using localStorage
- Responsive interface for desktop and mobile

## Run locally

Open `index.html` in a modern browser. For local development, a static server is also fine:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000.

## Publish with GitHub Pages

The included GitHub Actions workflow deploys the repository to GitHub Pages whenever changes are pushed to `main`.

If Pages has not been enabled for this repository yet, open **Settings → Pages** and select **GitHub Actions** as the build and deployment source. Then check the **Actions** tab for the first deployment.

## Notes

- Images selected as backgrounds stay on the user's device and are not uploaded.
- Google Fonts are loaded from Google Fonts; system fallbacks are provided if the service is unavailable.
- All rendering and PNG export happen in the browser.
