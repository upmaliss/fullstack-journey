## Day 5 — Inline, Block un Inline-Block elementi

### Block elementi

Aizņem visu rindas platumu. Sākas jaunā rindā.

Piemēri: div, p, h1-h6, ul, li, section, header

### Inline elementi

Aizņem tikai satura platumu. Paliek vienā rindā.
Nevar iestatīt width un height!

Piemēri: span, a, strong, em, img

### Inline-Block elementi

Paliek vienā rindā KĀ inline, bet var iestatīt
width un height KĀ block.

### Galvenā atšķirība

|                | Block | Inline     | Inline-Block |
| -------------- | ----- | ---------- | ------------ |
| Jauna rinda    | ✅    | ❌         | ❌           |
| Width/Height   | ✅    | ❌         | ✅           |
| Margin/Padding | ✅    | tikai sāni | ✅           |

### Svarīgi atcerēties

- display: block → padara inline par block
- display: inline → padara block par inline
- display: inline-block → labākais no abiem
