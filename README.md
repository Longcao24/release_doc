
- **API** — Major API generation (e.g., `1` = SATE API v1.x, `2` = SATE API v2.x)
- **FeatureMinor** — New features or non-breaking improvements
- **Patch** — Bug fixes and small polish

> Examples: `v1.0.0` (first on API v1), `v1.5.5` (feature & patches on API v1), `v2.0.0` (first on API v2)

Optional pre-release tags: `-alpha`, `-beta`, `-rc`.

---

## Release Timeline

### 🔹 v1.0 — Simple Reports & Conversation View
_7/10/2025_  
**New**
- Conversation transcript viewer  
- One-click **Simple Report** with basic analysis  
**Why it matters**
- Quick overview without setup  
- Baseline for future features

---

### 🔹 v1.5.5 — API v1.0 + Editing & Export
_8/15/2025_  
**New**
- **SATE API v1.0** integration  
- **Export (.txt)**: MLUm, MLUw, NTW, NDW, **List of Word Roots**  
- **Edit Mode** tools: edit text, change speaker, **merge/split** utterances, **annotate/exclude** segments  
- **Keyboard shortcuts**: `E` (Edit), `S` (Speaker), `M` (Merge), `/` (Split), `A` (Annotate/Exclude), `Esc` (Exit)  
**Why it matters**
- Faster transcript correction and review  
- Structured exports for downstream analysis

---

### 🔹 v1.5.8 — API v1.5 + Advanced Language Analysis + CRM Integration
**New**
- **SATE API v1.5** integration  
- **CRM system integration**: link session reports to client records; centralize transcripts, annotations, and metrics; reduce manual record-keeping  
- **Authenticated Core Language Metrics** *(all calculations exclude maze words such as repetitions, fillers, false starts, and revisions)*

**Syntax / Morphology**
- **MLUm** — Mean Length of Utterance (morphemes)  
- **MLUw** — Mean Length of Utterance (words)

**Semantics**
- **NTW** — Number of Total Words  
- **NDW** — Number of Different Words  
- **TTR** — Type–Token Ratio (NDW ÷ NTW)  
- **Moving-Average NTW** — window **100** (default), stride **1**  
- **Moving-Average NDW** — average NDW per window  
- **Moving-Average TTR** — MA-NDW ÷ MA-NTW  
- **VOCO-D (Lexical Diversity)** — prepared:  
  - N ∈ [35…50]  
  - For each N, compute Avg_TTR(N) from **100 random samples**  
  - Fit VOCD model to estimate **D**

**Verbal Fluency**
- **Pauses per Word**  
- **Words per Minute**  
- **Maze Words / Total Words**

**Quality of Life**
- **Spacebar** — Pause/Play audio  
- **Export (.txt)** — MLUm, MLUw, NTW, NDW, Word Roots

**Why it matters**
- Stronger reporting & tracking through CRM  
- Validated syntax/semantics/fluency metrics  
- Faster review via shortcuts and clean exports

---

## Keyboard Shortcuts

| Action                 | Key      |
|------------------------|----------|
| Play/Pause audio       | `Space`  |
| Edit segment           | `E`      |
| Change speaker         | `S`      |
| Merge utterances       | `M`      |
| Split utterance        | `P`      |
| Annotate / Exclude     | `A`      |
| Exit edit mode         | `Esc`    |

---

## Export Formats

- **Text (.txt)**: MLUm, MLUw, NTW, NDW, Word Roots  
- Encoding: **UTF-8**, newline-separated (spreadsheet-friendly)

---

## Metric Glossary

- **Maze words (excluded)** — fillers, repetitions, false starts, revisions, abandoned starts  
- **MLUm / MLUw** — average morphemes / words per utterance  
- **NTW / NDW** — total vs. unique lexical items  
- **TTR** — NDW ÷ NTW (lexical variety)  
- **Moving-Average metrics** — sliding window (default 100, stride 1)  
- **VOCO-D** — model-based estimate of lexical diversity using TTR vs. sample size

---

## Roadmap

- VOCO-D visualization with confidence bands  
- CSV/JSON export for all metrics  
- Custom window/stride settings  
- Per-speaker breakdowns

---

## Changelog (Chronological)

> Summarized list for quick scanning. See details above.

- **v1.5.8** — API v1.5; CRM integration; authenticated metrics; fluency metrics; spacebar playback; exports  
- **v1.5.5** — API v1.0; Edit Mode; `.txt` exports; keyboard shortcuts  
- **v1.0.0** — Simple report & conversation viewer

---

_Last updated: 10:00a 9/8/2025_
