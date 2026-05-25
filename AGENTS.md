# AGENTS.md

## Cursor Cloud specific instructions

This repository is a **pre-built static blog website** (Hexo 5.3.0 output with the Matery theme). It contains only the generated HTML/CSS/JS — no source Markdown, no `package.json`, no build tools.

### Running the site locally

```bash
python3 -m http.server 8080 --directory /workspace
```

Then open `http://localhost:8080/` in a browser. All pages (index, archives, categories, tags, about, individual posts) are served as static files.

### Key facts

- **No build step required** — the repo is the final static output.
- **No dependencies to install** — no `package.json`, `requirements.txt`, or similar files exist.
- **No lint/test/CI** — there are no automated tests, linters, or CI pipelines configured.
- **No backend services** — purely client-side HTML/CSS/JS.
- External features (Gitalk comments, Google Analytics) require network access and proper OAuth/API keys to function; they are non-essential for local development.
