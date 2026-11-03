# tools-web

Public frontend for small personal tools.

| Tool | Path | Data |
|------|------|------|
| 任务清单 | [`/todo/`](./todo/) | Private repo `jsl210101/tools-data` → `todo/tasks.json` |

## Notes

- Pages are public; **do not** put secrets or private task text into this repo.
- The todo page reads/writes `todo/tasks.json` in the private `tools-data` repo using a token the user pastes in the browser (stored only in `localStorage`).
- Live site: https://jsl210101.github.io/tools-web/

## Add a new tool

1. Put static files under `/<tool-name>/index.html`
2. Link it from `/index.html`
3. Keep private data in `tools-data`
