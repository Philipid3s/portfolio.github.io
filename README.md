# PoC Portfolio

Single-file static launchpad for proof-of-concept and prototype projects.

## Structure

- `index.html` contains the page markup, styles, project cards, and footer links.
- `robots.txt` and `sitemap.xml` provide basic crawler hints for search engines.
- `.nojekyll` keeps GitHub Pages in plain static-file mode.
- There is no build step or package manager dependency.
- The page is intended to run directly on GitHub Pages.

## Local Preview

Open `index.html` in a browser, or serve the directory locally:

```powershell
python -m http.server 8123
```

Then visit `http://127.0.0.1:8123/`.

## Editing Projects

Each project is an `<article class="card">` inside the `Project links` grid. Keep external links using:

```html
target="_blank" rel="noopener noreferrer"
```

This preserves safer behavior for links that open in a new tab.
