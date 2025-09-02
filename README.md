# Norway National Parks — External SVG Layers

This site uses **Map.svg** as the static basemap and **national_parks.svg** for park polygons/labels.
Click a park to toggle green + bold label. Light zoom (1×–4×).

## Run locally
```
python -m http.server 8080
# open http://localhost:8080/
```

## Deploy (GitHub Pages)
- Push the files in this folder to your repo root.
- Settings → Pages → Deploy from branch → (default branch) → root → Save.

## Input SVG summary
- Map.svg: viewBox = 0 0 774 774; shapes ~ 4378, texts ~ 0
- national_parks.svg: viewBox = 0 0 774 774; shapes ~ 41, texts ~ 0, titles ~ 0

If your parks SVG has no <text> labels, the page will generate labels from shape <title> or id and place them at each shape's bounding-box center.
