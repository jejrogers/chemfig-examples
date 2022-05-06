# LaTeX `chemfig` Package Examples

## Overview

I've made a bunch of `chemfig` examples because I often find the package confusing if it has been a while. I prefer it to ChemDraw et al., for drawing structures and reactions as it is free in both sense of the word.

I've done a bunch of customisation (visible in `config.tex`) to get the produced images looking like I want them too, which requires the **FreeSans** font (which requires `lualatex` to use). 

The `build` script is a `bash` script that automates the process of exporting the structures/schemes as `.svg` images for both light and dark backgrounds, as well as performing some organising and cleanup each time it is run. The script requires `pdf2svg`, `pdfcrop` and `sed`. 

## Examples

1. Structure of aripiprazole
2. Structure of venlafaxine with phenethylamine backbone indicated
3. Structure of MDMA with phenethylamine backbone indicated
4. Structure of escitalopram with stereochemistry indicated
5. A representative scheme of the pentadehydro Diels-Alder (PDDA) reaction

![](svg/light/01.svg#gh-light-mode-only)
![](svg/dark/01.svg#gh-dark-mode-only)

![](svg/light/02.svg#gh-light-mode-only)
![](svg/dark/02.svg#gh-dark-mode-only)

![](svg/light/03.svg#gh-light-mode-only)
![](svg/dark/03.svg#gh-dark-mode-only)

![](svg/light/04.svg#gh-light-mode-only)
![](svg/dark/04.svg#gh-dark-mode-only)

![](svg/light/05.svg#gh-light-mode-only)
![](svg/dark/05.svg#gh-dark-mode-only)
