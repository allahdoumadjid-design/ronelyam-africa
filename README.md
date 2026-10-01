# Ronelyam Africa

Static website for Ronelyam Africa. No Node.js dependencies or build step are required.

## Deploy on Vercel

1. Put the contents of this folder at the root of the GitHub repository, including `index.html`, `reference.css`, and the complete `assets/` directory.
2. Import that repository into Vercel.
3. Select **Other** as the framework preset.
4. Leave the build and install commands empty. Set the output directory to `.` if Vercel asks for one.
5. Deploy and verify the homepage, product images, WhatsApp links, and videos on the generated HTTPS URL.

The `assets/articles/` and `assets/videos/` folders are required. Keep their names and directory structure unchanged; the page builds media URLs from those paths.

## Test locally

From this folder, run a static HTTP server, for example:

```powershell
py -m http.server 8000
```

Then open `http://localhost:8000/` in a browser. Testing through HTTP also verifies video playback more reliably than opening `index.html` directly from disk.