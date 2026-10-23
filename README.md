# hermes-ppq-bootstrap

Static website that bootstraps a newcomer onto [Hermes Agent](https://hermes-agent.nousresearch.com/)
with [PayPerQ (ppq.ai)](https://ppq.ai) — pay-per-use, no subscription — using the
[ppq model-provider plugin](https://github.com/thepurpose-npub/ppq-hermes-provider) (v0.3.0).

## Live

Served by GitHub Pages from this repo (`main` root):

**https://thepurpose-npub.github.io/hermes-ppq-bootstrap/**

## Repo layout

- `index.html`, `style.css`, `.nojekyll` — the Pages content, served from
  `main` root (plain static files, no build step, no JS, no external requests).
  Pages source: Settings → Pages → "Deploy from a branch" → `main`, folder `/ (root)`.
- Local preview: `python3 -m http.server 8778` from this repo's root, then
  open http://localhost:8778/.
- This site deliberately lives in its own repo — the plugin repo
  (`thepurpose-npub/ppq-hermes-provider`) is sha-pinned by an open
  plugin-catalog PR and must not move HEAD for site edits.
- `local/` — local working history (handover briefs, deploy tars, archived
  drafts), gitignored via a single rule and not part of the site.

## Status

- **v1.0.0 (EN)** — content complete: 7 setup steps, cost-rail check,
  troubleshooting, and a collapsed "context & cost cheatsheet" section.
- **v1.1.0 (planned)** — German as default language, English as secondary.
