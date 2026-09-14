# Pepchem Pharmalabs — website

Single-file static website. `index.html` is the entire site (HTML, CSS, JavaScript,
fonts and images are all inside it). Three.js and GSAP load from cdnjs.

## How it goes live

    Claude (edits index.html) → GitHub (main branch) → Hostinger (auto-deploy) → live site

- Hostinger hPanel → Websites → Dashboard → Advanced → Git is connected to this
  repository, branch `main`, directory `public_html`.
- Every push/merge to `main` is deployed automatically. There is no build step.
- Do not rename `index.html` — it must sit at the repository root.

## Versions

Each accepted change is one commit. Use `git log` to see the history; the commit
message carries the build number (v12.xx) used in the working sessions.
