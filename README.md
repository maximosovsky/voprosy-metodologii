<div align="center">

# 📖 Voprosy Metodologii

![Scan sets](https://img.shields.io/badge/Scan_sets-15-8B4513?style=for-the-badge&logo=imagej&logoColor=white)
![JPG files](https://img.shields.io/badge/JPG_files-2274-D2691E?style=for-the-badge&logo=files&logoColor=white)
![Markdown texts](https://img.shields.io/badge/Markdown_texts-15-000000?style=for-the-badge&logo=markdown&logoColor=white)
![Period](https://img.shields.io/badge/Period-1991%E2%80%931999-556B2F?style=for-the-badge&logo=readthedocs&logoColor=white)

**A digital archive of the Russian journal Voprosy Metodologii (1991–1999).**

</div>

> Read the journal as machine-recognized text, check against the scanned pages, browse tables of contents in Markdown.

<div align="center">
  <a href="voprosy_metodologii_1991_1/0000.jpg"><img src="voprosy_metodologii_1991_1/0000.jpg" width="360" alt="Scanned cover from the 1991 No. 1 issue folder"></a>
  <br><br>
  <a href="#concept">Concept</a> · <a href="#features">Features</a> · <a href="#quick-start">Quick Start</a> · <a href="#catalog">Issue Catalog</a> · <a href="#tech-stack">Tech Stack</a> · <a href="#license">License</a> · <a href="#acknowledgements">Acknowledgements</a>
</div>

---

<a id="concept"></a>
## 💡 Concept

**Voprosy Metodologii** (Вопросы методологии, "Questions of Methodology") is a Russian-language methodological journal founded by Georgy Petrovich Shchedrovitsky. It was published under the aegis of the Committee for System-Thought-Activity Methodology and Organizational-Activity Games of the Union of Scientific and Engineering Societies (USSR), later as an independent journal of the methodological community. It published works of the Moscow Methodological Circle (MMK) and related fields: activity theory, SMD-methodology, pedagogy, organizational-activity games (ODI), systems approach, hermeneutics, and philosophy of economy.

This archive is for readers and researchers who need both machine-recognized text and the appearance of the printed source.

> [!NOTE]
> The repository contains **15 issue scan folders**, **2,274 JPG files**, **15 Markdown tables of contents** and **15 OCR texts in HTML**, covering the years 1991–1999 (1993 is missing).

---

<a id="features"></a>
## ✨ Features

| Feature | Description |
|---------|-------------|
| Original page images | Numbered JPG files preserve printed pages, covers and illustrations. |
| OCR texts | `pages.html` in each issue folder — full machine-recognized text. |
| Markdown tables of contents | One `.md` file per issue at the repo root: sections, authors, titles, page numbers. |
| Issue metadata | `meta.html` contains structured table of contents and imprint data. |
| Chronological catalog | Direct links to every scan folder and every table of contents, with JPG file counts. |
| LLM-readable documentation | `llms.txt` provides a short project card; `llms-full.txt` provides the full archive catalog with authors and articles. |

<details>
<summary>📚 Examples from the archive</summary>

| Issue | Examples from its contents |
|-------|----------------------------|
| [1991 No. 3](voprosy_metodologii_1991_3.md) | G. P. Shchedrovitsky — "Thinking through schemas of multiple knowledges"; I. S. Ladenko — "Formation and development of genetic logic ideas"; S. L. Frank — "An outline of the methodology of social sciences". |
| [1992 No. 1/2](voprosy_metodologii_1992_1-2.md) | G. P. Shchedrovitsky — "The natural and the artificial in socio-technical systems"; S. V. Naumov — "Conceptions of programs and programming in the context of methodological work". |
| [1994 No. 3/4](voprosy_metodologii_1994_3-4.md) | An issue dedicated to the memory of G. P. Shchedrovitsky: articles by Yu. V. Gromyko, O. I. Genisaretsky, V. M. Rozin and others. |
| [1996 No. 3/4](voprosy_metodologii_1996_3-4.md) | O. I. Genisaretsky — "Navigator: methodological extensions"; V. L. Glazychev — "Cultural policy". |
| [1999 No. 1/2](voprosy_metodologii_1999_1-2.md) | V. G. Bogin — "Several aspects of the problem of school education"; G. P. Shchedrovitsky — "The fate of the Tuesday seminar". |

These examples describe the source contents, not newly added interpretations or English translations.

</details>

---

<a id="quick-start"></a>
## 🚀 Quick Start

**Read on GitHub:** open [1991 No. 3 in Markdown](voprosy_metodologii_1991_3.md) or browse its [scan folder](voprosy_metodologii_1991_3/). The [catalog below](#catalog) links to the rest of the archive.

**Download the text and ToC collection with Git:**

```bash
git clone --depth=1 --filter=blob:none --sparse https://github.com/maximosovsky/voprosy-metodologii.git
cd voprosy-metodologii
git sparse-checkout set '*.md' '*.html' llms.txt llms-full.txt
```

Open a `.md` file with a Markdown viewer or text editor. `pages.html` opens in a browser.

<details>
<summary>🖼️ Include scans or download the entire archive</summary>

To include a specific issue's scans in a sparse checkout:

```bash
git sparse-checkout set '*.md' '*.html' llms.txt llms-full.txt voprosy_metodologii_1991_1
```

To expand an existing sparse checkout to all files:

```bash
git sparse-checkout disable
```

A conventional full clone is also possible:

```bash
git clone https://github.com/maximosovsky/voprosy-metodologii.git
```

Downloading all scans transfers substantially more data (~2 GB).

</details>

> [!TIP]
> Search across `pages.html` in a text editor to find names or concepts. Check important quotations against the corresponding scan — page numbers in `meta.html` and the `.md` tables of contents match JPG filenames.

---

<a id="catalog"></a>
## 🗂️ Issue Catalog

Issue names follow the folder names exactly. A JPG file may be a cover, a printed page or an additional image; the last column is not a printed-page count.

<details>
<summary>📑 All 15 scan sets · 15 ToCs · 2,274 JPG files</summary>

| Year | Issue | Scans | ToC | JPG |
|------|-------|-------|-----|-----|
| 1991 | No. 1 | [Scans](voprosy_metodologii_1991_1/) | [Read](voprosy_metodologii_1991_1.md) | 114 |
| 1991 | No. 2 | [Scans](voprosy_metodologii_1991_2/) | [Read](voprosy_metodologii_1991_2.md) | 114 |
| 1991 | No. 3 | [Scans](voprosy_metodologii_1991_3/) | [Read](voprosy_metodologii_1991_3.md) | 118 |
| 1991 | No. 4 | [Scans](voprosy_metodologii_1991_4/) | [Read](voprosy_metodologii_1991_4.md) | 114 |
| 1992 | No. 1/2 | [Scans](voprosy_metodologii_1992_1-2/) | [Read](voprosy_metodologii_1992_1-2.md) | 178 |
| 1992 | No. 3/4 | [Scans](voprosy_metodologii_1992_3-4/) | [Read](voprosy_metodologii_1992_3-4.md) | 162 |
| 1994 | No. 1/2 | [Scans](voprosy_metodologii_1994_1-2/) | [Read](voprosy_metodologii_1994_1-2.md) | 162 |
| 1994 | No. 3/4 | [Scans](voprosy_metodologii_1994_3-4/) | [Read](voprosy_metodologii_1994_3-4.md) | 178 |
| 1995 | No. 1/2 | [Scans](voprosy_metodologii_1995_1-2/) | [Read](voprosy_metodologii_1995_1-2.md) | 130 |
| 1996 | No. 1/2 | [Scans](voprosy_metodologii_1996_1-2/) | [Read](voprosy_metodologii_1996_1-2.md) | 130 |
| 1996 | No. 3/4 | [Scans](voprosy_metodologii_1996_3-4/) | [Read](voprosy_metodologii_1996_3-4.md) | 178 |
| 1997 | No. 1/2 | [Scans](voprosy_metodologii_1997_1-2/) | [Read](voprosy_metodologii_1997_1-2.md) | 162 |
| 1997 | No. 3/4 | [Scans](voprosy_metodologii_1997_3-4/) | [Read](voprosy_metodologii_1997_3-4.md) | 178 |
| 1998 | No. 1/2 | [Scans](voprosy_metodologii_1998_1-2/) | [Read](voprosy_metodologii_1998_1-2.md) | 178 |
| 1999 | No. 1/2 | [Scans](voprosy_metodologii_1999_1-2/) | [Read](voprosy_metodologii_1999_1-2.md) | 178 |

</details>

> [!NOTE]
> 1993 is missing — the journal was not published that year.

---

<a id="tech-stack"></a>
## 🏗️ Tech Stack

| Component | Technology |
|-----------|------------|
| Scans | JPEG (1200×2168 px) |
| Metadata | HTML (`meta.html` — structured table of contents) |
| OCR texts | HTML (`pages.html` — recognized text by page) |
| Tables of contents | Markdown (`.md` at root — sections, authors, pages) |
| Storage and history | Git / GitHub |
| Reading | GitHub, Markdown viewer, browser |

<details>
<summary>📁 Repository structure</summary>

```text
voprosy-metodologii/
├── voprosy_metodologii_1991_1/     # Scans and OCR
│   ├── 0000.jpg … 0113.jpg         (114 JPG)
│   ├── meta.html                   (table of contents)
│   └── pages.html                  (OCR text)
├── voprosy_metodologii_1991_2/
│   └── …
├── …
├── voprosy_metodologii_1999_1-2/
│   └── …
├── voprosy_metodologii_1991_1.md   # Table of contents in Markdown
├── voprosy_metodologii_1991_2.md
├── …
├── voprosy_metodologii_1999_1-2.md
├── llms.txt
├── llms-full.txt
├── README.md
└── LICENSE
```

- JPG filenames correspond to page numbers in `meta.html` and `.md` tables of contents.
- `pages.html` contains the full OCR text of the issue; recognition quality depends on the source.

</details>

---

<a id="contributing"></a>
## 🤝 Contributing

Fork → `fix/issue-description` → Pull Request.

For a text correction, identify the issue, the page number and the corresponding scan. If a missing issue is supplied, include its provenance and update the catalog and both LLM reference files.

---

<a id="license"></a>
## 📄 License

[Maxim Osovsky](https://www.linkedin.com/in/osovsky/). Licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).

> Archive of the journal. Copyright in the original texts belongs to their authors. Scanning and preparation of the archive — Maxim Osovsky.

---

<a id="acknowledgements"></a>
## 🙏 Acknowledgements

Our deep gratitude to V. M. Busev, founder of the [Electronic Library "Mathematical Education"](https://www.mathedu.ru/) (2018), for invaluable help with scanning, text recognition, hosting and support of the project.
