# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

See [README.md](README.md) for the full project overview, collection contents, and reading order.

## Working With This Repository

- `books/` contains 24 directories, each named for an apocryphal text
- Each directory has a `README.md` with scholarly context and a listing of available translation files
- Translation files are in PDF, Markdown (.md), or HTML format
- Markdown files are best for search, analysis, and text processing; PDFs preserve scholarly formatting
- `books.json` is the machine-readable index: it lists every file with its path, format, edition, translator, source and rights. Read it rather than inferring anything from a filename -- the naming conventions are not consistent, and neither are the markdown layouts. It declares the chapter and verse patterns for each format.
- **Do not assume every text is public domain.** `NOTICE.md` records the basis file by file. Six files have unresolved rights and one (`Additions_to_Esther_Wycliffe.pdf`) is under CC BY-NC-ND 4.0. Two copyrighted translations were removed from this repository; do not restore them from git history.
- `LICENSE` (CC BY 4.0) covers only the material written for this repository -- the README essays, the retranslation samples, and the creative work in `books/Tobit/` -- not the translations
- Some files are not scripture: the `books/Wisdom of Solomon/samples/` retranslations, `books/Tobit/the_weight_of_prayers.*`, and the Daubney study of the Additions to Daniel. They are flagged `"scripture": false` in `books.json`
