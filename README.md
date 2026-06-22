# sentriq-demo-docs

Static hosting for the **Sentriq** demo tenant's synthetic web-source pages, served via
GitHub Pages. These pages back the "web source" documents in the demo Knowledge Base so
the Digital CSM's RAG citation links resolve to a real page.

- **All content is synthetic** — Sentriq is a fictional product. Pages carry
  `<meta name="robots" content="noindex">`.
- Pages are **generated**, not hand-edited here. Source of truth lives in the main repo at
  `backend/scripts/demo_tenant/assets/kb/md/*.md`; render with
  `kb_render.py --web-only` and copy `assets/kb/web_html/*.html` to this repo root.
- `.nojekyll` disables Jekyll so files serve verbatim.

Served at: https://statisfy-us.github.io/sentriq-demo-docs/
