# Portfolio

A static site. All content lives in `content.json`; `index.html` renders it.

## Publish on GitHub Pages
1. Create a repo named `YOUR-USERNAME.github.io` and upload these files to the root.
2. Settings > Pages > Deploy from branch > `main` / root.
3. Visit `https://YOUR-USERNAME.github.io`.

## Preview locally
`python3 -m http.server` in this folder, then open http://localhost:8000. (Opening index.html directly won't load the JSON.)

## Edit content
- **New writing sample:** add an object to `writing` (title, type, desc, url, tags). Link `url` to a PDF in a `/samples` folder or an external page.
- **New job:** add an object to `experience` (newest first).
- **New skill:** add `{ "name": "...", "tags": ["data"] }` to a group's `items`, or add a new group. Groups with no matching skills hide automatically.
- **New role filter:** add `{ "id": "x", "label": "..." }` to `lenses`, then use `"x"` in any item's `tags`.
- Replace the placeholder writing samples and the GitHub/LinkedIn links in `site.links`.
