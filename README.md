# ddd-models

3D doll GLB models (Draco-compressed) for the confinement-escape game on
https://donttalk.vercel.app/games/confinement-escape

Served to the site via jsDelivr CDN so the 51 models (~26 MB) do not count
against the Vercel Hobby 100 MB deployment upload limit:

```
https://cdn.jsdelivr.net/gh/123lai1234-create/ddd-models@v1/models/<id>.glb
```

- `models/<id>.glb` — one Draco GLB per character (51 total).
- Face textures are projected from the original card art; see the
  `donttalk` repo (`astro/scripts/patch-game-html.py`) for the viewer that
  loads these URLs.
- Do not delete or rename files under `models/` — the game page references
  them by id. New versions go out as a new tag (e.g. `v2`) and the viewer
  URL is updated to match.
