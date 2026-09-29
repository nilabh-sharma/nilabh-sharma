# Nilabh Sharma — Data, AI & Delivery

Educational site built with [MkDocs Material](https://squidfunk.github.io/mkdocs-material/).

## Run locally

```bash
python -m venv .venv && source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
mkdocs serve        # open http://127.0.0.1:8000
```

## Publish to GitHub Pages (one-time setup)

1. Create an empty **public** repo on GitHub named exactly `<your-username>.github.io` (e.g. `nilabhsharma.github.io`). This makes it your personal site, served at the root URL.
2. From this folder:
   ```bash
   git init && git add . && git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
   git push -u origin main
   ```
3. The included GitHub Action (`.github/workflows/deploy.yml`) builds the site on every push and publishes it to a `gh-pages` branch.
4. In the repo: **Settings → Pages → Source: Deploy from a branch → Branch: `gh-pages` / root → Save**.
5. Site is live at `https://<your-username>.github.io/` within a minute or two.
6. Uncomment `site_url` and `repo_url` in `mkdocs.yml` and set your username.

## Custom domain (optional)

1. Buy a domain (OVH, Cloudflare, Namecheap…).
2. Create `docs/CNAME` containing just your domain, e.g. `aifordataengineers.com`.
3. At your DNS provider, point the domain to GitHub Pages (see GitHub docs: "Managing a custom domain for your GitHub Pages site").
4. Settings → Pages → Custom domain → tick **Enforce HTTPS**.

## Writing a new article

1. Add a Markdown file under `docs/`, e.g. `docs/foundations/embeddings.md`.
2. Add it to `nav:` in `mkdocs.yml`.
3. `mkdocs serve` to preview, then commit and push — it deploys automatically.

Useful syntax: admonitions (`!!! note`), tabs, tables, code blocks, and Mermaid diagrams (```` ```mermaid ````).
