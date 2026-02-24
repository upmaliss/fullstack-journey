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

## Day 6 — Positioning un Pseudo Elements

### CSS Positioning

#### position: static (noklusējums)

Elements atrodas normālā dokumenta plūsmā.
Neviens offset (top, left utt.) nedarbojas.

#### position: relative

Elements paliek normālā plūsmā, bet var pārvietot
ar top, left, right, bottom — relatīvi pret savu
sākotnējo vietu.

#### position: absolute

Iziet no normālās plūsmas. Pozicionējas relatīvi
pret tuvāko vecāku ar position: relative.
Ja nav — tad relatīvi pret body.

#### position: fixed

Paliek ekrānā fiksēts — neritina ar lapu.
Lietojums: navigācija, cookie banner.

#### position: sticky

Ritina ar lapu līdz noteiktai vietai, tad paliek fiksēts.
Lietojums: navigācija kas "pielīp" augšā scrollojot.

### Svarīgi atcerēties

- absolute vienmēr vajag relative vecāku
- z-index strādā tikai ar pozicionētiem elementiem
- fixed un absolute iziet no normālās plūsmas

---

### Pseudo Elements

Pseudo elementi ļauj stilizēt **daļu no elementa**
vai pievienot saturu bez HTML izmaiņām.

#### ::before

Pievieno saturu PIRMS elementa.

#### ::after

Pievieno saturu PĒC elementa.

#### ::first-line

Stilizē tikai pirmo teksta rindu.

#### ::first-letter

Stilizē tikai pirmo burtu — piemēram laikrakstu stils.

#### ::selection

Stilizē tekstu kad to iezīmē ar peli.

### Svarīgi atcerēties

- ::before un ::after vienmēr vajag content: ""
- Tie ir daļa no elementa, ne atsevišķi HTML tagi
- Labi izmantot dekoratīviem elementiem
  lai HTML paliek tīrs
