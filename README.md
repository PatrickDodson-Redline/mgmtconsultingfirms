# Redline Growth, Management Consulting BD Microsite

A standalone static microsite for the Management Consulting segment. No build step, no framework, no dependencies to install. Pure HTML, CSS, and JavaScript.

## Structure

    index.html        The microsite. Open this first.
    assets/           Interactive panels the page loads as iframes
                      (dossier, signal library, value model, diagrams).
    .nojekyll         Tells GitHub Pages to serve files as-is.

All links are relative, so the package runs from any folder or repo path.

## Deploy to GitHub Pages

1. Push these files to a repository, with index.html at the repo root.
2. In the repository, open Settings, then Pages.
3. Under Build and deployment, choose Deploy from a branch, pick your branch, and set the folder to root.
4. Save, wait for the build, then open the Pages URL. index.html serves at the root.

## Preview locally

The page loads its panels as iframes. Some browsers block iframe content opened over the file protocol, so the most reliable local preview is a small static server:

    python3 -m http.server 8000

Then open http://localhost:8000 in a browser. Opening index.html directly will work in most browsers, but the static server avoids any iframe loading quirks.

## Notes

Fonts load from the Google Fonts CDN, so a network connection is needed for exact typography. Everything else is local. Example accounts, names, and figures are illustrative and fictional.
