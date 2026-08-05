# My Blog

A personal blog built with [Quarto](https://quarto.org) and hosted on **GitHub Pages**.

- Live site: https://geilehirnbude.github.io/notes-of-a-nerd/
- See [BLOG-CHEATSHEET.md](./BLOG-CHEATSHEET.md) for how to write/publish posts.

## Quick start

```bash
# Local preview
quarto preview
```

## Write a post

Drop a file in `posts/`:

- `posts/YYYY-MM-DD-title.qmd` — Markdown post (title, author, date, categories in YAML frontmatter)
- `posts/YYYY-MM-DD-title.ipynb` — Jupyter notebook, rendered natively (no conversion step)

It appears on the homepage automatically. Publish by committing and pushing to `main`:

```bash
git add -A && git commit -m "New post" && git push origin main
```

The GitHub Action (`.github/workflows/publish.yml`) builds the site and deploys to the `gh-pages` branch.

## Config

Site-wide settings live in [`_quarto.yml`](./_quarto.yml) (title, navbar, theme, bibliography).

Citations use [`references.bib`](./references.bib) natively.
