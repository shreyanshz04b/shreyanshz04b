# Validation checklist

- [x] SVG XML parsed successfully.
- [x] Unique ID check performed per SVG.
- [x] Original portrait and pointing-character PNG bytes embedded unchanged.
- [x] SVG assets use local data URIs and no external image/font requests.
- [x] README uses the five requested relative SVG paths with `?v=1`.
- [x] Project table retains all three projects and does not invent repository URLs.
- [x] Social links are ordinary Markdown links outside the SVGs.
- [x] Static fallback renders and a contact sheet were generated.
- [x] Local preview page uses `<img>` embedding at desktop and mobile widths.
- [ ] Timed browser renders at 0s, 2s, 5s, 9s, and 13s were not completed in this run.
- [ ] The requested per-SVG 1 MB and package 4 MB limits cannot be met simultaneously with byte-preserved source PNGs embedded inline in self-contained SVGs. See `validation.json`.
- [ ] GitHub's exact sanitizer/runtime behavior cannot be fully guaranteed by local SVG validation alone.
