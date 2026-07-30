# Apocryphal, Deuterocanonical & Pseudepigraphal Texts

A curated collection of 24 ancient religious writings related to but not included in the standard Protestant biblical canon. Each text lives in its own directory under `books/` with translations in multiple formats (PDF, Markdown, HTML) and a detailed README covering sources, history, summary, themes, and legacy.

For programmatic use, [`books.json`](books.json) is a machine-readable index of every file in the collection: path, format, edition, translator, source, and rights basis. It also flags the files that are *not* scripture and should not be served as such.

## The Collection

### Phase 1: Deuterocanonical Core
*Included in Catholic and Orthodox Bibles. Start here.*

| # | Text | Description |
|---|------|-------------|
| 1 | [Wisdom of Solomon](books/Wisdom%20of%20Solomon/) | Philosophical meditation on wisdom and righteousness; bridges Hebrew and Greek thought |
| 2 | [Sirach](books/Sirach/) | Practical wisdom literature; the longest deuterocanonical book |
| 3 | [Tobit](books/Tobit/) | Narrative of faith, family, and angelic intervention; accessible storytelling |
| 4 | [Judith](books/Judith/) | Heroic narrative of a woman saving her people |
| 5 | [Baruch](books/Baruch/) | Short prophetic text attributed to Jeremiah's scribe |
| 6 | [1 Maccabees](books/1%20Maccabees/) | Historical account of the Maccabean revolt (175-134 BCE); essential for understanding Second Temple Judaism |
| 7 | [2 Maccabees](books/2%20Maccabees/) | Theological interpretation of the same period; introduces resurrection theology |
| 8 | [Additions to Esther](books/Additions%20to%20Esther/) | Greek expansions adding prayer and divine action to the Esther narrative |
| 9 | [Additions to Daniel](books/Additions%20to%20Daniel/) | Three additions: Prayer of Azariah, Susanna, and Bel and the Dragon |
| 10 | [1 Esdras](books/1%20Esdras/) | Greek retelling of the return from exile, containing the Debate of the Three Guardsmen -- "Great is truth, and mighty above all things" |
| 11 | [2 Esdras](books/2%20Esdras/) | Seven visions of Ezra arguing with an archangel about why God permits the wicked to prosper; the source of the Requiem's *requiem aeternam* |
| 12 | [Prayer of Manasseh](books/Prayer%20of%20Manasseh/) | Fifteen verses of penitence attributed to Judah's worst king; a canticle in the Book of Common Prayer |

### Phase 2: Pseudepigrapha and Apocalyptic Literature
*Shaped early Jewish and Christian cosmology.*

| # | Text | Description |
|---|------|-------------|
| 13 | [1 Enoch](books/1%20Enoch/) | Foundational apocalyptic text; the Watchers, heavenly visions, Son of Man prophecies. Quoted in Jude. |
| 14 | [2 Enoch](books/2%20Enoch/) | Enoch's ascent through the heavens; more mystical than 1 Enoch |
| 15 | [Jubilees](books/Jubilees/) | Retelling of Genesis-Exodus with a 364-day solar calendar and expanded angelic lore |
| 16 | [Life of Adam and Eve](books/Life%20of%20Adam%20and%20Eve/) | Post-Eden narrative; Satan's origin story and the promise of resurrection |
| 17 | [Testament of Solomon](books/Testament%20of%20Solomon/) | Solomon commanding demons; origin of Solomonic magical tradition |

### Phase 3: New Testament Apocrypha and Gnostic Texts
*Reveal the diversity of early Christianity.*

| # | Text | Description |
|---|------|-------------|
| 18 | [Gospel of James](books/Gospel%20of%20James/) | The Protoevangelium; Mary's childhood and the nativity. Very influential in Christian art and Mariology. |
| 19 | [Gospel of Thomas](books/Gospel%20of%20Thomas/) | 114 sayings of Jesus; no narrative, pure logia. Compare with the Synoptic Gospels. |
| 20 | [Gospel of Mary](books/Gospel%20of%20Mary/) | Mary Magdalene as spiritual leader; early debates about women's authority |
| 21 | [Gospel of Philip](books/Gospel%20of%20Philip/) | Gnostic sacramental theology; the "bridal chamber" mystery |
| 22 | [Gospel of Judas](books/Gospel%20of%20Judas/) | Sethian Gnostic cosmology; Judas as Jesus' most trusted disciple |
| 23 | [Acts of Paul and Thecla](books/Acts%20of%20Paul%20and%20Thecla/) | Early Christian adventure narrative; a woman as apostolic figure |
| 24 | [Apocalypse of Peter](books/Apocalypse%20of%20Peter/) | Visions of heaven and hell; influenced Dante and medieval eschatology |

## Translation Sources

Translations sourced from:

- **eBible.org** -- King James Version with Apocrypha, World English Bible, Revised Version, and LXX2012
- **Project Gutenberg** -- Douay-Rheims translations (from the Latin Vulgate)
- **Wikisource** -- proofread transcriptions of R. H. Charles's 1 Enoch and of 2 Enoch
- **pseudepigrapha.com** -- R. H. Charles's Jubilees, from *The Apocrypha and Pseudepigrapha of the Old Testament* (1913)
- **Internet Archive / sacred-texts.com** -- various scholarly editions and PDFs
- **earlychristianwritings.com / New Advent** -- Roberts-Donaldson and other Ante-Nicene Fathers translations
- **gospels.net** -- Mark M. Mattison's public domain translations of the Gnostic gospels

## Rights

Almost every translation here is in the public domain, but **not all of them**, and the difference matters if you are redistributing the collection:

- [`NOTICE.md`](NOTICE.md) records, file by file, the specific basis for each translation's status -- a quoted dedication, or a translator and publication date. It also lists six files whose rights could not be established, and one file (`Additions_to_Esther_Wycliffe.pdf`) that is under copyright and distributed under CC BY-NC-ND 4.0.
- [`LICENSE`](LICENSE) covers the original material written for this repository -- the per-book README essays, the retranslation samples, and the creative work in `books/Tobit/` -- under CC BY 4.0. It makes no claim over the translations.
- Every file in [`books.json`](books.json) carries its own `rights` object, so a consumer can filter on it rather than trusting a blanket claim.

## Reading the Texts

Each book directory contains:
- **README.md** -- Source manuscripts, historical context, canonical status, full summary, key themes, and influence/legacy
- **Translation files** -- One or more translations in PDF, Markdown, or HTML. Markdown files are best for reading and search; PDFs preserve scholarly formatting.

Markdown files do not all share one layout -- the collection draws on several sources, and each keeps its own conventions. `books.json` declares the format of every file explicitly, with the chapter and verse patterns for each, so you do not have to sniff it. Every markdown file is UTF-8 with LF line endings, so those patterns match whether you read a checkout or fetch the raw file over HTTP.

Two texts are awkward to read straight: the Apocalypse of Moses carries its chapter and verse numbers inside the running prose, and the Apocalypse of Peter interleaves M. R. James's introduction and notes with the four texts he translates. Both now have a companion file, named in the manifest as `derivedFile`, holding the translation on its own in a format the manifest already defines. Neither changes a word of the translation, and the original file remains the edition of record. Where a file's structure could only be described by hand -- which part of it is translation and which is the translator's own matter -- the manifest records that too, under `structure`.

The [Wisdom of Solomon](books/Wisdom%20of%20Solomon/samples/) directory also contains sample retranslations of Chapter 1 in four styles: modern plain English, literary modern English, narrative storytelling, and annotated modern English. These are AI-generated adaptations, not translations, and are flagged `"scripture": false` in the manifest.
