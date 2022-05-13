# LaTeX `chemfig` Package Examples

## Overview

I've made a bunch of `chemfig` examples because I often find the package confusing if it has been a while. I prefer it to ChemDraw et al., for drawing structures and reactions as it is free in both sense of the word.

I've done a bunch of customisation (visible in `config.tex`) to get the produced images looking like I want them too, which requires the **FreeSans** font (which requires `lualatex` to use). 

The `build` script is a `bash` script that automates the process of exporting the structures/schemes as `.svg` images for both light and dark backgrounds, as well as performing some organising and cleanup each time it is run. The script requires `pdf2svg`, `pdfcrop` and `sed`. 

## Current Examples (More to Come...)

1. Structure of aripiprazole

   ![](svg/light/01.svg#gh-light-mode-only)

   ![](svg/dark/01.svg#gh-dark-mode-only)

2. Structure of venlafaxine with phenethylamine backbone indicated

   ![](svg/light/02.svg#gh-light-mode-only)

   ![](svg/dark/02.svg#gh-dark-mode-only)

3. Structure of escitalopram with stereochemistry indicated

   ![](svg/light/03.svg#gh-light-mode-only)

   ![](svg/dark/03.svg#gh-dark-mode-only)

4. A representative scheme of the tetradehydro Diels-Alder (TDDA) reaction

   ![](svg/light/04.svg#gh-light-mode-only)

   ![](svg/dark/04.svg#gh-dark-mode-only)

5. Diacetyl ferrocene structure

   ![](svg/light/05.svg#gh-light-mode-only)

   ![](svg/dark/05.svg#gh-dark-mode-only)

6. Structure of NMDA receptor antagonist memantine

   ![](svg/light/06.svg#gh-light-mode-only)

   ![](svg/dark/06.svg#gh-dark-mode-only)

7. A transition metal complex with counterions (Ru(bpy3)Cl2)

   ![](svg/light/07.svg#gh-light-mode-only)

   ![](svg/dark/07.svg#gh-dark-mode-only)
