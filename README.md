# Singenuity Competitor Playbook (hosted)

Static, self-contained training site for the SDR team. `index.html` is generated from
`competitors/battlecards.md` by `scripts/build_competitor_views.py` — do not hand-edit it.

## Deploy (GitHub Pages)
1. Create a new **public** repo (e.g. `competitor-playbook`).
2. Copy everything in this folder (`index.html`, `.nojekyll`, `robots.txt`, this README) to the repo root; commit + push.
3. Repo → **Settings → Pages** → Source: *Deploy from a branch* → Branch: `main` / `/root` → Save.
4. Wait ~1 min; the URL appears at the top of the Pages settings. Share that link in Slack.

## Update
Re-run `scripts/build_competitor_views.py`, copy the new `index.html` over, commit + push. Pages redeploys automatically.

> Note: GitHub Pages on a free account is public. `noindex` + `robots.txt` keep it out of search, but anyone with the link can view it. For a gated version, host behind Cloudflare Access instead.
