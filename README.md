# Project Website Starter

This repository now contains only the files required to build and publish the project website with [MkDocs Material](https://squidfunk.github.io/mkdocs-material/).

## Directory overview

- `docs/` — Markdown pages, images, and other assets that appear on the site.
- `mkdocs.yml` — Site navigation and theme configuration.
- `requirements.txt` — Python dependencies for building the site locally or in CI.

## Editing the site

1. Update the Markdown files inside `docs/` to change page content.
2. Adjust the navigation or theme settings in `mkdocs.yml` as needed.
3. Commit and push your changes. If GitHub Pages is configured to deploy from the `/docs` directory on the `main` branch, the site will rebuild automatically.

## Preview locally

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
mkdocs serve
```

Then open the URL printed in the terminal (usually http://127.0.0.1:8000/) to preview the site.

## Deploying with GitHub Pages

1. Go to **Settings → Pages**.
2. Set **Source** to **Deploy from a branch**.
3. Choose the `main` branch and the `/docs` folder.
4. Save. GitHub will provide the public URL for your site.

With this lean setup you can focus entirely on crafting the website content for your new project.
