# GitHub Pages homepage

A small personal homepage built with **plain HTML and CSS — no dependencies, no build step**.
It is made to live at the root of a repository named
`YOUR-USERNAME.github.io`, so GitHub Pages serves it at
`https://YOUR-USERNAME.github.io/`.

## Files

| File         | Purpose                                              |
| ------------ | ---------------------------------------------------- |
| `index.html` | The page content (hero, about, learning, projects).  |
| `styles.css` | All styling: layout, colors, responsive + dark theme.|

There are no `node_modules`, no lockfile, and no third-party assets, so nothing
has to be installed.

## Preview locally

Pick whichever is easiest.

### Option A — just open the file (simplest)

Double-click `index.html`, or run:

```bash
# macOS
open index.html

# Windows (PowerShell)
start index.html

# Linux
xdg-open index.html
```

### Option B — a tiny local server (closer to GitHub Pages)

From inside this folder, run one of:

```bash
# Python 3 (installed on most machines)
python3 -m http.server 8000

# or, if you have Node.js
npx serve .
```

Then open <http://localhost:8000> in your browser. Stop the server with `Ctrl + C`.

## Publish on GitHub Pages

1. Create a **public** repository named exactly `YOUR-USERNAME.github.io`
   (use your real GitHub username). On GitHub Free it must be public.
2. Upload `index.html` and `styles.css` to the repository **root**.
   You can drag-and-drop them with *Add file → Upload files*, or use Git:

   ```bash
   git init
   git add index.html styles.css README.md
   git commit -m "Add personal homepage"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/YOUR-USERNAME.github.io.git
   git push -u origin main
   ```

3. Wait a minute (the very first build can take a few minutes), then open
   `https://YOUR-USERNAME.github.io/`.
4. If it does not appear, check **Settings → Pages** and make sure the source is
   the `main` branch, folder `/ (root)`.

## Make it yours

Search `index.html` for `TODO(you)` and edit:

- the `<title>` and meta description,
- the name "Alex" and the one-line introduction,
- the "About", "Learning", and "Projects" text,
- the two GitHub links (`profile-link` and `contact-github`) — point them at
  `https://github.com/YOUR-USERNAME`.

Colors are changed in one place: the variables at the top of `styles.css`.
Keep `index.html` at the repository root, otherwise Pages will not serve it at the
bare `https://YOUR-USERNAME.github.io/` URL.

> Privacy: this template contains no student ID, homework details, or private
> information. Review the text before publishing — a Pages site is public.
