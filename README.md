# LaTeX `chemfig` Package Examples

## Motivation

I've made a bunch of `chemfig` examples because I often find the package
confusing if it has been a while. I prefer it to ChemDraw et al., for drawing
structures and reactions as it is free in both sense of the word.

Each file is commented with some descriptions and explanations on how things
were achieved.

## Operation and Requirements

I've done a bunch of customisation (visible in `config.tex`) to get the produced
images looking like I want them too, which requires the **FreeSans** font (which
requires `lualatex` to use). 

The `build` script is a `bash` script that automates the process of exporting
the structures/schemes as `.svg` images for both light and dark backgrounds, as
well as performing some organising and cleanup each time it is run. The script
requires `pdf2svg`, `pdfcrop` and `sed`. 

## Current Examples (More to Come...)

### Organic and Drug-Like Molecules

1. Aripiprazole

   ![](svg/light/01.svg#gh-light-mode-only)

   ![](svg/dark/01.svg#gh-dark-mode-only)

2. Venlafaxine showing the phenethylamine backbone

   ![](svg/light/02.svg#gh-light-mode-only)

   ![](svg/dark/02.svg#gh-dark-mode-only)

3. Escitalopram

   ![](svg/light/03.svg#gh-light-mode-only)

   ![](svg/dark/03.svg#gh-dark-mode-only)

4. Memantine

   ![](svg/light/06.svg#gh-light-mode-only)

   ![](svg/dark/06.svg#gh-dark-mode-only)

5. Quetiapine

   ![](svg/light/09.svg#gh-light-mode-only)

   ![](svg/dark/09.svg#gh-dark-mode-only)

6. Scopolamine

   ![](svg/light/10.svg#gh-light-mode-only)

   ![](svg/dark/10.svg#gh-dark-mode-only)

7. 8-Chlorotheophylline

   ![](svg/light/11.svg#gh-light-mode-only)

   ![](svg/dark/11.svg#gh-dark-mode-only)

8. Myristicin

   ![](svg/light/12.svg#gh-light-mode-only)

   ![](svg/dark/12.svg#gh-dark-mode-only)

9. Benzydamine

   ![](svg/light/13.svg#gh-light-mode-only)

   ![](svg/dark/13.svg#gh-dark-mode-only)

10. Coronene/Superbenzene

    ![](svg/light/14.svg#gh-light-mode-only)

    ![](svg/dark/14.svg#gh-dark-mode-only)

### Polymers

1. Homopolymer polystyrene

   ![](svg/light/08.svg#gh-light-mode-only)

   ![](svg/dark/08.svg#gh-dark-mode-only)

### Inorganic Compounds

1. Ferrocene derivative

   ![](svg/light/05.svg#gh-light-mode-only)

   ![](svg/dark/05.svg#gh-dark-mode-only)

2. Ir(ppy)3

   ![](svg/light/07.svg#gh-light-mode-only)

   ![](svg/dark/07.svg#gh-dark-mode-only)

### Reaction Mechanisms

1. Cycloaddition reaction (tetradehydro Diels-Alder (TDDA))

   ![](svg/light/04.svg#gh-light-mode-only)

   ![](svg/dark/04.svg#gh-dark-mode-only)

2. Decarboxylation of cyclic peroxyester to excited ketone

   ![](svg/light/15.svg#gh-light-mode-only)

   ![](svg/dark/15.svg#gh-dark-mode-only)

3. Nucleophilic aromatic substitution reaction

   ![](svg/light/16.svg#gh-light-mode-only)

   ![](svg/dark/16.svg#gh-dark-mode-only)
