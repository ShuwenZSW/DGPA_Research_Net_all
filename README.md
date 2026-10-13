# DGPA Research Net — All Members

A shared, self-updating map of research themes, methods and regions across all 22 DGPA faculty (Public Administration, International Relations, and Political Science) — built to make collaboration opportunities visible.

**Open the app:** https://shuwenzsw.github.io/DGPA_Research_Net_all/

## How it works

- **Similarity view** — who shares research ground with whom (theme / method / region, weighted).
- **Complementarity view** — pairs with genuinely different topics who still share a primary method and a primary region (so collaboration is realistic). Complementarity Index (CI, 0–10) = 2×theme distance + method overlap + 0.75×region overlap, normalized; shown only when CI ≥ 7.5 and theme distance ≥ 0.6. Anyone without a qualifying pair keeps their single closest feasible match, drawn lighter and marked "nearest match" — so no one is isolated.
- **Edit My Profile tab** — every member keeps their own topics, methods, regions and interests current, and emails the changes to the map maintainer.
- **Site Feedback tab** — comments about the website itself go to the same address.

## Two modes

- **Static (GitHub Pages, the link above):** edits are saved in your own browser as a local preview. To publish them for everyone, click *Save (local demo only)* then *Email changes* in the Edit tab — the maintainer merges the update and republishes the shared data.
- **Live (LAN):** run `python3 server.py` in this folder and share `http://<machine-ip>:8000` on the department network — edits then sync between everyone automatically (the page detects the server and switches mode by itself).

## Data

`data.json` holds all profiles and the theme/method/region label sets. Coding: 48 fine-grained themes / 8 methods / 8 regions; primary (●) vs secondary (○) weights; 14 theme domains (node colors). Source: faculty webpages + Google Scholar profiles (2026-10-13), to be confirmed and adjusted by each member.
