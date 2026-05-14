# NotebookLM Video Package — *Beam or Be Left Behind*

English-language cinematic video resources for the essay *"Beam or Be Left Behind: A Slovenian Plan to Skip Digital Transformation and Jump Straight Into AI"*.

## Files

| File | Purpose |
|---|---|
| `01-essay.md` | **Primary source.** The full essay — the spine of the video. |
| `02-data-and-sources.md` | Every verified figure (Eurostat, SURS, WEF, OECD, Microsoft WorkLab, e-Estonia, Klarna) with citation links. The video must not invent numbers. |
| `03-blockers-and-cliff.md` | The psychology of adoption: the three-week cliff, the permission gap, the compounding gap — the *why* behind the six blockers. |
| `04-moment-of-joy.md` | The "beaming" concept (Singhal), the Celje metalworking-firm vignette as the human anchor. |
| `05-references-estonia-finland.md` | Estonia's AI Leap and Finland's phenomenon-based learning as concrete reference models. |
| `notebooklm-prompt.md` | **Director's brief.** The cinematic customize prompt for NotebookLM Video Overview. Under 2.5 KB to stay inside NotebookLM's customize-field limit. |
| `youtube-description.md` | Publish-ready YouTube description with timestamps to fill in after the final cut. |

## Workflow

1. Open [NotebookLM](https://notebooklm.google.com/) and create a new notebook named *"Beam or Be Left Behind — Slovenia AI Plan"*.
2. Upload **all five** `0X-*.md` files as sources. Make `01-essay.md` the highest-priority source (NotebookLM lets you weight or pin).
3. Generate **Video Overview**. In the *Customize* field, paste the contents of `notebooklm-prompt.md` verbatim.
4. On first generation, verify:
   - Numbers are exact (22%, 18%, 72%, ~54 points, 20%, 60%, 28%, €18–28M, 180–280k seats).
   - Celje is named and used as a vignette.
   - The three-act structure (diagnosis → "beaming" → six moves) is intact.
   - Closing lands on "tomorrow morning" — quiet, not bombastic.
5. Regenerate with prompt tweaks if pronunciation, pacing, or emphasis drifts.
6. Upload to YouTube using `youtube-description.md`. Fill in the timestamp placeholders against the actual cut.

## Target

- **Language:** English. (Slovenian-language version intentionally not included in this round.)
- **Style:** cinematic documentary — register of *NYT Op-Docs*, *BBC Storyworks*, *Bloomberg Originals*. Not a podcast. Not a marketing explainer.
- **Length:** 7–9 minutes.
- **Audience:** Slovenian executives, education leaders, civil servants, policymakers; secondary audience: EU policy readers and international observers of small-country AI strategy.

## Quality bar

**Exact:** every number used in the narration must come from `02-data-and-sources.md`. No hallucinated figures, no "industry surveys say…" filler.

**Engaging:** the Celje vignette is the human spine — return to it. The pacing has tension (the diagnosis) and release (the joy moment) before the plan. The closing is quiet.
