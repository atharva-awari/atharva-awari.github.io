# Personal website

A single static page (`index.html`) with its images and fonts in `assets/`. It needs no build step, no Jekyll and no Ruby.

## Put it online with GitHub Pages

1. Create a public repository named exactly `<your-username>.github.io`.
2. Upload the contents of this folder (`index.html`, `assets/`, this README) to the repository root.
3. In the repository, open **Settings → Pages**, set **Source** to "Deploy from a branch", choose `main` and `/ (root)`, and save.
4. After a minute the site is live at `https://<your-username>.github.io`.

To use your own domain later, add it under **Settings → Pages → Custom domain** and point a DNS record at GitHub, as their documentation describes.

## Before going live

- **Photo:** save a square photo as `assets/img/photo.jpg` and replace the `<div class="portrait">AA</div>` block in `index.html` with the `<img>` line in the comment just above it.
- **CV:** save your CV as `assets/cv.pdf`. The "Download CV" button already points there.
- **Profile links:** fill in Google Scholar, ORCID and LinkedIn in the commented block under the GitLab link, and remove the comment markers.
- **Email:** the page shows your UMONS address. Switch it to an address that will outlive the move to SimulaMet.

## Updating

- **New paper:** copy one `<li>` in the Publications section and edit it. The "Cite" button is a `<details>` block holding the BibTeX.
- **News:** add a line at the top of the News list. Use `class="cell up"` for something upcoming and `class="cell"` once it has happened.
- **Banner animation:** it is drawn by the script at the bottom of `index.html`. The factor sizes (`m`, `n`, `p`, `r`) and the loop timing (`LOOP` and `state()`) are at the top of that script.

Fonts: STIX Two Text and Public Sans, self-hosted under the SIL Open Font License (see `assets/fonts`).
