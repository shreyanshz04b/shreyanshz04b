# Verification report

## Structural checks

- **PASS** — `hero.svg`: valid XML; 6 IDs; duplicate IDs=[]; external references=False; embedded PNG data URIs=2; 4,263,751 bytes.
- **PASS** — `about-life.svg`: valid XML; 6 IDs; duplicate IDs=[]; external references=False; embedded PNG data URIs=0; 8,231 bytes.
- **PASS** — `stack.svg`: valid XML; 3 IDs; duplicate IDs=[]; external references=False; embedded PNG data URIs=0; 7,139 bytes.
- **PASS** — `id-dashboard.svg`: valid XML; 8 IDs; duplicate IDs=[]; external references=False; embedded PNG data URIs=1; 2,475,848 bytes.
- **PASS** — `connect.svg`: valid XML; 3 IDs; duplicate IDs=[]; external references=False; embedded PNG data URIs=1; 1,541,224 bytes.

## Identity asset integrity

- **PASS** — `id.png` byte-identical to supplied file; 1,849,967 bytes; SHA-256 `c5ef46759266f29111dd9ca76d76bd329b8e00ae77fb3d585e5d81ae0bd9efe0`.
- **PASS** — `right_pointing.png` byte-identical to supplied file; 1,150,625 bytes; SHA-256 `c389e6ca2783cfe1ddbb1db25d1c4be362cbcc976f1ae44592f7805630299728`.
- **PASS** — `signature.png` byte-identical to supplied file; 1,341,692 bytes; SHA-256 `545fbb36b1b02213fadb15b6e2cfe452f33e356c39691e77b8436cd0e165ed32`.

## README and package checks

- **PASS** — all 11 supplied social URLs appear in README Markdown.
- **PASS** — all five SVGs referenced with `?v=1`; original signature used for closing sign-off.
- **PASS** — badge animation now separates the drop translation from the clasp-centred pendulum rotation.
- **NOT TESTED** — animated frames at 0, 2, 5, 9, and 13 seconds. CairoSVG does not execute CSS/SMIL animation; Playwright Chromium is not installed in this environment.
- **NOT TESTED** — live GitHub rendering, URL ownership, and link reachability.
- **NOT TESTED** — licensed WOFF2 font embedding; system font stacks are used for offline rendering.
- **Static renders:** 5/5 generated and included in the contact sheet.
- **Package source tree size:** 13,463,526 bytes.
- **SIZE BUDGET CONFLICT:** The three supplied PNGs alone total 4,342,284 bytes before SVG base64 embedding or any code. Since the original files must remain byte-identical and images must be embedded in self-contained SVGs, the requested 4 MB total package limit is mathematically incompatible with the other requirements. Originals were not altered or lossily optimized.

## Notes

- Signature PNG is opaque white-background artwork as supplied; no transparency is claimed.
- GitHub metrics are omitted because no verified metrics were supplied.
- The ID badge is labelled as a personal profile concept, not an official credential.
- Static screenshots verify layout only; exact animation timing still requires a browser-capable test.
