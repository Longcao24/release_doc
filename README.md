# 🚀 SATE — Release Notes & Changelog

## Release Timeline

### 🔹 v1.5.8 — Advanced Language Analysis + CRM Integration (API v1.5)  
_Released: 9/8/2025_

**New**
- CRM system integration: link session reports to client records, centralize transcripts and metrics  
- Advanced language metrics *(excluding maze words like fillers, repetitions, false starts)*:  
  - **Syntax/Morphology**: MLUm, MLUw  
  - **Semantics**: NTW, NDW, TTR, moving-average NTW/NDW/TTR, VOCO-D (lexical diversity, prepared)  
  - **Verbal Fluency**: pauses per word, words per minute, maze words/total words  
- Quality of life:  
  - `Spacebar` = play/pause audio  
  - Export metrics to `.txt`  

**Why it matters**
- Stronger client tracking with CRM  
- Clinically validated measures of syntax, semantics, and fluency  
- Faster review with shortcuts and improved exports

---

### 🔹 v1.5.5 — Editing & Export (API v1.0)  
_Released: 8/15/2025_

**New**
- Export to `.txt`: MLUm, MLUw, NTW, NDW, **List of Word Roots**  
- Edit Mode: edit text, change speaker, merge/split utterances, annotate/exclude segments  
- Keyboard shortcuts:  
  - `E` (Edit)  
  - `S` (Speaker)  
  - `M` (Merge)  
  - `P` (Split)  
  - `A` (Annotate/Exclude)  
  - `Esc` (Exit)  

**Why it matters**
- Faster transcript correction and cleanup  
- Structured exports for research and reports

---

### 🔹 v1.0 — Simple Reports & Conversation View  
_Released: 7/10/2025_

**New**
- Conversation transcript viewer  
- One-click **Simple Report** with basic analysis  

**Why it matters**
- Quick overview of sessions without setup  
- Foundation for future analysis features

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

- **Maze words** — fillers, repetitions, false starts, abandoned starts  
- **MLUm / MLUw** — average morphemes / words per utterance  
- **NTW / NDW** — total vs. unique words  
- **TTR** — lexical diversity (NDW ÷ NTW)  
- **Moving-Average metrics** — calculated with sliding window (default 100, stride 1)  
- **VOCO-D** — statistical model of lexical diversity  

---

## Roadmap

- VOCO-D visualization with confidence bands  
- CSV/JSON export for all metrics  
- Custom window/stride settings  
- Per-speaker breakdowns

---

## Changelog (Quick View)

- **v1.5.8** — CRM integration, advanced metrics, fluency, exports, playback  
- **v1.5.5** — Edit Mode, `.txt` export, keyboard shortcuts  
- **v1.0.0** — Conversation viewer, simple report

---

_Last updated: 10:00 AM · 9/8/2025_
