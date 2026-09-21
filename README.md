# Penrose Cup Rulebook

Official Penrose Cup competition rulebook for EA SPORTS F1 26, built with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).

## Run locally

```sh
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
mkdocs serve
```

Open the local URL shown by MkDocs. Use `mkdocs build --strict` before committing.

## Content and navigation

Rule pages are in `docs/section-one` through `docs/section-five`; add or edit regulation text in the relevant individual Markdown page. Add a page to the `nav` section of `mkdocs.yml` to show it in the rulebook sidebar. Branding artwork is `docs/assets/penrose-cup.png`, and theme styling lives in `docs/stylesheets/extra.css`.

## Deployment

Pushing `main` runs `.github/workflows/deploy.yml`, which builds and deploys to GitHub Pages. In the repository's **Settings → Pages**, set the source to **GitHub Actions** once.
