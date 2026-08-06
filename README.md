Job search results repository

Replaces `jobsearch_results` (2026-08-06): that repo's GitHub Pages deployment got
stuck in a way that persisted across every fix attempted from the client/API side
(retries, a self-controlled Actions workflow, disable+re-enable) — five consecutive
deployments all hung at `deployment_queued` and timed out. This repo starts fresh
with its own GitHub Pages environment; content is otherwise identical.

Deployed automatically by `.github/workflows/pages.yml` on every push to `main`.
Source content lives in the private `jobsuche-2026` repo; this repo is a generated
mirror, safe to regenerate from scratch at any time.
