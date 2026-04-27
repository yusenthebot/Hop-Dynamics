# Prompt: Design a "Much Better" Academic Research Poster

Use the following rules to produce a high-quality academic research poster. Follow every rule unless I explicitly override one.

---

## RULE 0 — CANVAS & FORMAT
- **Physical size: 48 in × 36 in (1219 mm × 914 mm), landscape orientation, 4:3 aspect ratio.** This is the US conference standard; the nearest ISO equivalent is **A0 landscape (1189 mm × 841 mm, also 4:3-ish)**. If I specify "ISO" explicitly, use **A0 landscape (1189 × 841 mm)**. If I specify "A1", use **A1 landscape (841 × 594 mm)**.
- Export at **300 DPI** for print, plus a low-res PDF preview.
- Bleed: 0.25 in safe margin inside the edge; no text or critical figure content closer than 0.5 in to any edge.

## RULE 1 — GRID & LAYOUT
- Use a **3-column grid** with 0.4–0.6 in gutters between columns. Columns should be roughly equal width (~15 in each for a 48 in canvas).
- **Center column is the hero zone**: place the single most important figure (system diagram, pipeline, or key result) here, sized to span most of the vertical height.
- **Left column = context**: Abstract → Motivation → Goals/Aims (top to bottom).
- **Right column = outcomes**: Results → Supporting modules/details → Future Work → Acknowledgements → References (top to bottom).
- Reading order must flow **top→bottom within a column, then left→right across columns**. Never force the reader to hunt.

## RULE 2 — TITLE BANNER (TOP STRIP, ~8% OF POSTER HEIGHT)
- Title: one sentence, **60–80 pt bold**, sentence case or title case, centered. Must describe the contribution, not just the topic.
- Author row directly below title: **24–28 pt**, with superscript affiliation numbers.
- Affiliation row below authors: **18–22 pt italic or regular**, single line if possible.
- **Institution logo on top-left**, **funder/lab/collaborator logos on top-right**. Logos sized to match title row height; do not let logos overpower the title.

## RULE 3 — SECTION HEADERS
- Every section gets a **solid-color filled bar** (full column width) with **white text, 32–40 pt bold, left-aligned**. Use the accent color defined in Rule 7.
- Section header bar height: ~0.6–0.8 in. Consistent across every section.
- **No underlines, no thin accent lines** under titles — use the filled bar instead.

## RULE 4 — KEY-TAKEAWAY CALLOUT BARS (the "Much Better" trick)
- Under each Results or major Methods subsection, insert a **colored horizontal callout bar** (same accent color, lighter tint or with opacity) containing **one plain-English takeaway sentence in 20–26 pt bold italic**.
- Examples: *"Individual tools maintain high fidelity in mm-scale geometries."* / *"Automated tool transitions enable printing of complex composite structures."*
- Reader should be able to understand the poster's conclusions by reading **only these callout bars + the title**. This is the single most important rule.

## RULE 5 — BODY TEXT
- Body font size: **22–28 pt** (never below 20 pt — remember it will be read from 3–6 ft away).
- Max line length: ~10–14 words per line; never run text across the full 48 in width.
- **No walls of text.** Each paragraph ≤ 4 lines. Prefer bulleted lists with tight 3–6 word bullets over prose where possible.
- **Left-align all body text.** Center-align only titles, section headers, and figure captions.
- Line spacing: 1.15–1.25.

## RULE 6 — FIGURES
- **One dominant hero figure** in the center column at 80–100% column width.
- Every figure must have: **(a)** a numbered caption starting with *Fig. N.* in **14–18 pt**, **(b)** a **scale bar** with numeric label (e.g., "10 mm") burned into the image when the figure shows physical objects/microscopy, and **(c)** labeled sub-panels (A, B, C…) if the figure has multiple views.
- Figures must be **≥ 300 DPI at final print size** — no visible pixelation when zoomed to 100% print scale.
- Annotate figures directly (callout letters A/B/C/D/E/F) and reference those letters in the adjacent body text.

## RULE 7 — COLOR PALETTE
- **One dominant color** (60–70% of visual weight) for section headers + callout bars. Default: use the lead institution's brand color (e.g., CMU red `#C41230`, Stanford `#8C1515`, MIT `#750014`).
- **One neutral background**: white or very light warm gray (`#F7F4EE` or `#FFFFFF`).
- **Two supporting tones** max: black/dark charcoal for body text, one muted secondary (gray `#4A4A4A`) for captions.
- **Never use more than 4 colors total.** No rainbow callouts. No drop shadows. No gradients on text.

## RULE 8 — TYPOGRAPHY PAIRING
- **Headers/Title**: a confident serif or bold humanist sans (e.g., *Georgia Bold*, *Calibri Bold*, *Source Sans Pro Black*, *Merriweather Bold*).
- **Body**: a clean neutral sans (e.g., *Calibri*, *Source Sans Pro*, *Helvetica Neue*, *Open Sans*).
- **Never mix more than two font families.** No Comic Sans, no Papyrus, no decorative fonts.

## RULE 9 — WHITESPACE & ALIGNMENT
- Minimum 0.3 in gap between any two content blocks; 0.5 in preferred.
- Every element must snap to the 3-column grid or to a shared horizontal baseline with its neighbors. Nothing should appear "floating" or rotated off-axis.
- Leave ~5% of the poster as deliberate empty space — do not fill every square inch.

## RULE 10 — REFERENCES, ACKNOWLEDGEMENTS, QR CODE
- References: bottom of right column, **compressed single block in 12–14 pt**, numbered `[1], [2], …` and cited inline in the body as superscripts or bracketed numbers.
- Acknowledgements: one line naming the funder + grant number (e.g., *"This work was supported by ARO Cooperative Agreement W911NF-23-2-0138"*).
- **Include a QR code** (0.8–1.2 in square, high contrast, black on white) in a bottom corner linking to the paper/preprint/lab page. Label it with 14 pt text: "Paper & code" or similar.

## RULE 11 — HIERARCHY CHECK (mandatory self-review)
Before declaring the poster done, verify by squinting / standing back 6 ft:
1. Can a reader grasp the main finding in **≤ 10 seconds** by reading only the **title + callout bars**? If no, rewrite the callouts.
2. Is there exactly **one** visual focal point in the center? If multiple elements compete, demote all but one.
3. Does every section header use the **same color, same height, same font size**? If not, unify.
4. Are all figures **≥ 300 DPI** and do they all have **scale bars + numbered captions**?
5. Is body text **≥ 20 pt** everywhere (even references footnote style stays readable at 12–14 pt)?
6. Is the color palette **≤ 4 colors**?

## RULE 12 — THINGS TO AVOID
- Do not use clip-art, stock photos of "diverse researchers looking at screens," or generic AI-generated illustrations.
- Do not center-align body paragraphs.
- Do not use underlines to indicate emphasis (use bold or color).
- Do not use drop shadows, glows, 3D bevels, or WordArt.
- Do not repeat the abstract verbatim in the body — the abstract is the short version; the body sections expand different parts of it.
- Do not exceed **~800 words total** across the entire poster.

---

## OUTPUT FORMAT I EXPECT FROM YOU
When I give you content to put on a poster, return:
1. A layout plan (which block goes where on the 3-column grid, with approximate in/cm dimensions).
2. The exact text for the title, authors, each section header, each callout-bar takeaway, body copy, and figure captions.
3. A color palette with hex codes.
4. A font pairing recommendation.
5. A QR-code target URL (ask me if missing).
6. The final deliverable as **either a PPTX file sized 48×36 in, or a print-ready PDF at 300 DPI**, whichever I request.
