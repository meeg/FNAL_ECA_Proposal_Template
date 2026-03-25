# FNAL ECA Proposal Template

This repository facilitates the combination of user content with central style and formatting provided by FNAL.

Users should enter content in the following locations (items 4-8 cover the required appendices):
1. [info.tex](./info.tex): details for cover page
2. [packages.tex](./packages.tex): any additional packages used
3. [content.tex](./content.tex): the actual proposal content
4. [biblio.tex](./biblio.tex): references
5. [facilities.tex](./facilities.tex): facilities
6. [equipment.tex](./equipment.tex): equipment
7. [dataplan.tex](./dataplan.tex): data management plan
8. [other.tex](./other.tex): other attachments (e.g. letters of collaboration using the `\collabletter{}` command)

## References
The template is set up to use BibLaTeX+Biber, with the bibliogrpahy generated automatically from records that you dump in [references.bib](./references.bib).
If you prefer, by commenting/uncommenting code in [biblio.tex](./biblio.tex) you can opt to format your bibliography manually, with entries that you list in the `\thebibliography` block in that file.

## Compilation

For standalone use, basic compilation is as simple as (if using Biber):
```bash
pdflatex main.tex
biber main
pdflatex main.tex
```

or (if manually formatting the bibliography):
```bash
pdflatex main.tex
```

Depending on your use of references, bibliography tools, etc., you may need to run `pdflatex` and/or `biber` multiple times (following cues from the compilation messages).

This repository can also be used as a base to create new projects on [Overleaf](https://overleaf.com).
There are several methods for this:
1. New Project -> Import from GitHub (requires linking your GitHub account)
2. Upload Project (download [zip file](https://github.com/kpedro88/FNAL_ECA_Proposal_Template/archive/refs/heads/main.zip))

This repository is set up on GitHub as a "template repository", so you can create your own repository based on it *without* needing to make a public fork, if desirable.
