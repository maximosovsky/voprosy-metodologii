<div align="center">

# 📖 Вопросы методологии

![Scan sets](https://img.shields.io/badge/Scan_sets-15-8B4513?style=for-the-badge&logo=imagej&logoColor=white)
![JPG files](https://img.shields.io/badge/JPG_files-2274-D2691E?style=for-the-badge&logo=files&logoColor=white)
![Markdown texts](https://img.shields.io/badge/Markdown_texts-15-000000?style=for-the-badge&logo=markdown&logoColor=white)
![Period](https://img.shields.io/badge/Period-1991%E2%80%931999-556B2F?style=for-the-badge&logo=readthedocs&logoColor=white)

**Цифровой архив журнала «Вопросы методологии» (1991–1999).**

</div>

> Читайте журнал как распознанный текст, сверяйтесь со сканами страниц, изучайте оглавления в Markdown.

<div align="center">
  <a href="voprosy_metodologii_1991_1/0000.jpg"><img src="voprosy_metodologii_1991_1/0000.jpg" width="360" alt="Обложка №1, 1991"></a>
  <br><br>
  <a href="#concept">Концепция</a> · <a href="#features">Возможности</a> · <a href="#quick-start">Быстрый старт</a> · <a href="#catalog">Каталог</a> · <a href="#tech-stack">Состав</a> · <a href="#license">Лицензия</a>
</div>

---

<a id="concept"></a>
## 💡 Концепция

**«Вопросы методологии»** — журнал методологического сообщества, основанный Г. П. Щедровицким. Выходил под эгидой Комитета по системомыследеятельностной методологии и организационно-деятельностным играм, затем — как независимый журнал методологического сообщества. Публиковал работы Московского методологического кружка (ММК) и смежных направлений: теория деятельности, СМД-методология, педагогика, ОДИ, системный подход, герменевтика, философия хозяйства.

Архив предназначен для читателей и исследователей, которым нужен и распознанный текст, и облик печатного источника.

> [!NOTE]
> Репозиторий содержит **15 папок со сканами**, **2274 JPG-файла**, **15 оглавлений в Markdown** и **15 OCR-текстов в HTML**. Охвачены годы 1991–1999 (1993 отсутствует).

---

<a id="features"></a>
## ✨ Возможности

| Возможность | Описание |
|-------------|----------|
| Оригинальные сканы | Пронумерованные JPG-файлы сохраняют печатные страницы, обложки и иллюстрации. |
| OCR-тексты | `pages.html` в каждой папке выпуска — полный распознанный текст. |
| Оглавления в Markdown | По одному `.md`-файлу на выпуск в корне репозитория: рубрики, авторы, названия, страницы. |
| Метаданные выпуска | `meta.html` содержит структурированное содержание и выходные данные. |
| Хронологический каталог | Прямые ссылки на каждую папку сканов и каждое оглавление, с числом JPG-файлов. |
| Документация для LLM | `llms.txt` — короткая карточка проекта; `llms-full.txt` — полный каталог всех выпусков с авторами и статьями. |

<details>
<summary>📚 Примеры из архива</summary>

| Выпуск | Примеры содержания |
|--------|---------------------|
| [1991 № 3](voprosy_metodologii_1991_3.md) | Г. П. Щедровицкий — «Мышление по схемам многих знаний»; И. С. Ладенко — «Становление и развитие идей генетической логики»; С. Л. Франк — «Очерк методологии общественных наук». |
| [1992 № 1/2](voprosy_metodologii_1992_1-2.md) | Г. П. Щедровицкий — «Естественное и искусственное в социотехнических системах»; С. В. Наумов — «Представления о программах и программировании». |
| [1994 № 3/4](voprosy_metodologii_1994_3-4.md) | Номер памяти Г. П. Щедровицкого: статьи Ю. В. Громыко, О. И. Генисаретского, В. М. Розина и др. |
| [1996 № 3/4](voprosy_metodologii_1996_3-4.md) | О. И. Генисаретский — «Навигатор: методологические продолжения»; В. Л. Глазычев — «Культурная политика». |
| [1999 № 1/2](voprosy_metodologii_1999_1-2.md) | В. Г. Богин — «Несколько аспектов проблемы школьного образования»; Г. П. Щедровицкий — «Судьба вторничного семинара». |

Описания передают содержание источников, а не добавленные интерпретации.

</details>

---

<a id="quick-start"></a>
## 🚀 Быстрый старт

**Читать на GitHub:** откройте [1991 № 3 в Markdown](voprosy_metodologii_1991_3.md) или просмотрите [папку сканов](voprosy_metodologii_1991_3/). [Каталог ниже](#catalog) содержит ссылки на весь архив.

**Скачать только текст и оглавления через Git:**

```bash
git clone --depth=1 --filter=blob:none --sparse https://github.com/maximosovsky/voprosy-metodologii.git
cd voprosy-metodologii
git sparse-checkout set '*.md' '*.html' llms.txt llms-full.txt
```

Откройте `.md`-файл в любом редакторе Markdown. `pages.html` открывается в браузере.

<details>
<summary>🖼️ Включить сканы или скачать весь архив</summary>

Чтобы добавить сканы конкретного выпуска в sparse checkout:

```bash
git sparse-checkout set '*.md' '*.html' llms.txt llms-full.txt voprosy_metodologii_1991_1
```

Чтобы расширить существующий sparse checkout до всех файлов:

```bash
git sparse-checkout disable
```

Полный клон:

```bash
git clone https://github.com/maximosovsky/voprosy-metodologii.git
```

Загрузка всех сканов передаёт значительно больше данных (~2 GB).

</details>

> [!TIP]
> Ищите по `pages.html` в текстовом редакторе, чтобы находить имена и понятия. Сверяйте важные цитаты с соответствующим сканом — номера страниц в `meta.html` и `.md`-оглавлениях соответствуют номерам JPG-файлов.

---

<a id="catalog"></a>
## 🗂️ Каталог выпусков

Названия выпусков следуют именам папок. JPG-файл может быть обложкой, печатной страницей или вложением; последний столбец не является подсчётом печатных страниц.

<details>
<summary>📑 Все 15 выпусков · 15 оглавлений · 2274 JPG-файла</summary>

| Год | Выпуск | Сканы | Оглавление | JPG |
|-----|--------|-------|------------|-----|
| 1991 | № 1 | [Сканы](voprosy_metodologii_1991_1/) | [Читать](voprosy_metodologii_1991_1.md) | 114 |
| 1991 | № 2 | [Сканы](voprosy_metodologii_1991_2/) | [Читать](voprosy_metodologii_1991_2.md) | 114 |
| 1991 | № 3 | [Сканы](voprosy_metodologii_1991_3/) | [Читать](voprosy_metodologii_1991_3.md) | 118 |
| 1991 | № 4 | [Сканы](voprosy_metodologii_1991_4/) | [Читать](voprosy_metodologii_1991_4.md) | 114 |
| 1992 | № 1/2 | [Сканы](voprosy_metodologii_1992_1-2/) | [Читать](voprosy_metodologii_1992_1-2.md) | 178 |
| 1992 | № 3/4 | [Сканы](voprosy_metodologii_1992_3-4/) | [Читать](voprosy_metodologii_1992_3-4.md) | 162 |
| 1994 | № 1/2 | [Сканы](voprosy_metodologii_1994_1-2/) | [Читать](voprosy_metodologii_1994_1-2.md) | 162 |
| 1994 | № 3/4 | [Сканы](voprosy_metodologii_1994_3-4/) | [Читать](voprosy_metodologii_1994_3-4.md) | 178 |
| 1995 | № 1/2 | [Сканы](voprosy_metodologii_1995_1-2/) | [Читать](voprosy_metodologii_1995_1-2.md) | 130 |
| 1996 | № 1/2 | [Сканы](voprosy_metodologii_1996_1-2/) | [Читать](voprosy_metodologii_1996_1-2.md) | 130 |
| 1996 | № 3/4 | [Сканы](voprosy_metodologii_1996_3-4/) | [Читать](voprosy_metodologii_1996_3-4.md) | 178 |
| 1997 | № 1/2 | [Сканы](voprosy_metodologii_1997_1-2/) | [Читать](voprosy_metodologii_1997_1-2.md) | 162 |
| 1997 | № 3/4 | [Сканы](voprosy_metodologii_1997_3-4/) | [Читать](voprosy_metodologii_1997_3-4.md) | 178 |
| 1998 | № 1/2 | [Сканы](voprosy_metodologii_1998_1-2/) | [Читать](voprosy_metodologii_1998_1-2.md) | 178 |
| 1999 | № 1/2 | [Сканы](voprosy_metodologii_1999_1-2/) | [Читать](voprosy_metodologii_1999_1-2.md) | 178 |

</details>

> [!NOTE]
> 1993 год отсутствует — в этот год журнал не выходил.

---

<a id="tech-stack"></a>
## 🏗️ Состав архива

| Компонент | Технология |
|-----------|------------|
| Сканы | JPEG (1200×2168 px) |
| Метаданные | HTML (`meta.html` — структурированное содержание) |
| OCR-тексты | HTML (`pages.html` — распознанный текст по страницам) |
| Оглавления | Markdown (`.md` в корне — рубрики, авторы, страницы) |
| Хранение и история | Git / GitHub |
| Чтение | GitHub, редактор Markdown, браузер |

<details>
<summary>📁 Структура репозитория</summary>

```text
voprosy-metodologii/
├── voprosy_metodologii_1991_1/     # Сканы и OCR
│   ├── 0000.jpg … 0113.jpg         (114 JPG)
│   ├── meta.html                   (оглавление)
│   └── pages.html                  (OCR-текст)
├── voprosy_metodologii_1991_2/
│   └── …
├── …
├── voprosy_metodologii_1999_1-2/
│   └── …
├── voprosy_metodologii_1991_1.md   # Оглавление в Markdown
├── voprosy_metodologii_1991_2.md
├── …
├── voprosy_metodologii_1999_1-2.md
├── llms.txt
├── llms-full.txt
├── README.md
└── LICENSE
```

- Номера JPG-файлов соответствуют номерам страниц в `meta.html` и `.md`-оглавлениях.
- `pages.html` содержит полный OCR-текст выпуска; качество распознавания зависит от источника.

</details>

---

<a id="contributing"></a>
## 🤝 Участие

Fork → `fix/описание-правки` → Pull Request.

Для текстовой правки укажите выпуск, номер страницы и соответствующий скан. При добавлении пропущенного выпуска приложите информацию о происхождении и обновите каталог и оба LLM-файла.

---

<a id="license"></a>
## 📄 Лицензия

[Maxim Osovsky](https://www.linkedin.com/in/osovsky/). Licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).

> Архив журнала. Авторские права на оригинальные тексты принадлежат их авторам. Оцифровка и подготовка архива — Maxim Osovsky.