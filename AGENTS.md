# AGENTS.md

## Cursor Cloud specific instructions

### Project Overview

This repository is a **pre-built static Hexo blog** (the compiled output of a Hexo 5.3.0 project). It contains only rendered HTML, CSS, JS, and media assets — there is no build system, no `package.json`, no dependency manifest, and no source Markdown files in this repo.

### Running the Site

Serve the repository root with any static HTTP server:

```bash
cd /workspace && python3 -m http.server 8080
```

Then open `http://localhost:8080/` in a browser. All pages (archives, categories, tags, about, individual posts) are pre-rendered and served as static files.

### Key Notes

- **No dependencies to install.** There is no `package.json`, `requirements.txt`, or any package manifest.
- **No build step.** The HTML/CSS/JS is already compiled and ready to serve.
- **No linting or tests.** There are no lint configs or test frameworks present.
- **Assets use absolute paths** (e.g. `/css/matery.css`, `/libs/jquery/jquery.min.js`), so the server must serve from the repository root.
- The blog uses the **hexo-theme-matery** theme with Materialize CSS, jQuery, lightGallery, and other vendored libraries.
- Comment systems (Gitalk, Valine) and analytics (Google Analytics, busuanzi) reference external services and may not function in local development.
