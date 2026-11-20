# SAFE-DR demo website

Static site (no build step). Open `index.html` locally or deploy to GitHub Pages.

## Deploy to GitHub Pages
1. Create a public repo named `SAFE-DR` and upload the contents of this `site/` folder (keep `index.html` at the repo root).
2. Settings → Pages → Source: *Deploy from a branch* → `main` / `(root)`.
3. The site appears at `https://wilop272.github.io/SAFE-DR/`.

## Files
| File | Purpose |
| --- | --- |
| `index.html` | Project page: motivation, embedded demo video, method, results, interactive replay, limitations |
| `demo.mp4` | 59 s recorded pipeline replay (also embedded in the PPT) |
| `demo_anim.html` | Source animation for the video; open `demo_anim.html?autoplay` to replay it live in a browser |
| `assets/replay.js` | Archived probe/head weights and 199 cached external rows for the in-browser SAFE-DR port |
| `assets/results.js` | `reproduced_tables.json` produced by `python evaluate.py` |
| `assets/architecture.png` | **Add your architecture figure here.** If it is missing, the page shows a text pipeline instead |

## Placeholders to replace
- `Group [X]` and `Member A–E` in `index.html` (hero, team section, footer)
- Report / Colab / Code button links (`href="#"`) in the hero

## Honesty notes (already shown on the page)
- The demo is a **recorded replay** of real cached rows (IDRiD #346, #62; EyePACS #1207, #231). The cache contains no original images.
- Fundus photos are public illustrative images (CC0 / NEI public domain / CC BY 4.0). Lesion overlays come from a classical top-hat filter, not from D²-Mamba.
