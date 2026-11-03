# tools-web

Public frontend for small personal tools.

| Tool | Path | Data |
|------|------|------|
| 任务清单 | [`/todo/`](./todo/) | Private repo `jsl210101/tools-data` → `todo/tasks.json` |

## Live site

Intended URL: https://jsl210101.github.io/tools-web/

If that 404s, enable Pages once (the deploy PAT may lack Pages permission):

1. Open https://github.com/jsl210101/tools-web/settings/pages
2. Build and deployment → Source: **Deploy from a branch**
3. Branch: **main** / folder: **/ (root)** → Save

## Notes

- Pages are public; **do not** put secrets or private task text into this repo.
- The todo page reads/writes `todo/tasks.json` in private `tools-data` using a token the user pastes in ⚙ 同步设置 (stored only in browser `localStorage`).
- Without a token the page shows only the setup prompt (no task titles).

## Add a new tool

1. Put static files under `/<tool-name>/index.html`
2. Link it from `/index.html`
3. Keep private data in `tools-data`
