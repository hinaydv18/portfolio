# Hina Yadav – Data & BI Analyst Portfolio

Static site (no build step, no dependencies). Bilingual EN/FR with a language toggle.

## Pages (hash routes in `index.html`)

| Route | Page |
|---|---|
| `#/` | Accueil — headline, key figures, project list |
| `#/parcours` | Mon parcours — career timeline, OpenClassrooms certification, languages |
| `#/projets` | Projets — all six projects + skills matrix |
| `#/p/<id>` | Project detail (nba, ins, crm, csat, bn, bi) with slides and source-file download |
| `#/competences` | Compétences — skills by area + per-project matrix |
| `#/hobbies` | Hobbies |
| `#/cv` | CV — download the 4 PDFs + previews |
| `#/contact` | Contact — email, phone, LinkedIn, GitHub |

## Folder layout (important — do not remove)

- `index.html` — the whole site (content is in the `P`, `XP`, `HB`… lists inside the script)
- `assets/<project>/1.jpg …` — project screenshots (graphs). Missing folder = broken images.
- `files/` — downloadable source files (.pptx, .pbix, .ipynb). Missing folder = broken downloads.
- `cv-fr.jpg`, `cv-en.jpg`, `Hina_YADAV_CV_*.pdf` — CV previews and downloads

## Publish on GitHub Pages

The repo already has a Pages workflow (`.github/workflows/static.yml`) that deploys the
repository root on every push to `main`. So: commit everything (including `assets/` and
`files/`), push to `main`, and the site updates at https://hinaydv18.github.io/portfolio/.

## Edit

- Contact links: `CONTACT` at the top of the `<script>` in `index.html`.
- Texts (English and French): the `o("English","Français")` pairs.
- Projects: the `P` list. Career timeline: the `XP` list. Hobbies: the `HB` list.
- Power BI screenshots: add `assets/bi/1.png`, `2.png`… and captions in the `im:[]` list of the `bi` project.
