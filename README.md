# LaTeX `chemfig` Package Examples

## Motivation

I've made a bunch of `chemfig` examples because I often find the package confusing if it has been a while. I prefer it to ChemDraw et al., for drawing structures and reactions as it is free in both sense of the word (and because I'm broke and no longer affiliated with an academic organisation).

I also enjoy the more "programmatic" approach to creating structures as they can easily be fine-tuned, duplicated, tweaked, etc. with nothing but a text editor.

Each file is commented with some descriptions and explanations on how things were achieved. This is not currently as comprehensive as I would like it to be, however, so feel free to email/message me with any questions or assistance requests :)

## Operation and Requirements

I've done a bunch of customisation (visible in `config.tex`) to get the produced images looking like I want them to.

Some of these configurations include:

* The optional use of the **FreeSans** font, which is freely available and permissively licensed. The font is easily changed to any system fonts picked up by `lualatex`
    * Optionally `pdflatex` can be used instead and a font package (e.g. `mathptmx`, `arev`, etc.) can be used
* A 12 pt font size, with most other measurements defined using em and ex, to scale cleanly when the font size is changed
* A base angle increment of 30º to easily facilitate the 60º angles standard in typical chemical drawings
* Custom widths for the wedge and dashed bonds and a custom bond length to look clean and familiar
* Some predefined element colours that will adjust brightness whether the drawing is in dark or light mode, to keep things legible
    * Note that colouring the atoms is done manually and hence entirely optional
* Some custom commands to simplify styling conditions in reaction schemes and floating stereochemistry markers -- i.e. *(S)*, *(R)*, *(E)*, *(Z)*, etc.

The `build` script is a `bash` script that automates the process of exporting the structures/schemes as `.svg` images for both light and dark backgrounds, as well as performing some organising and cleanup each time it is run. The script requires `pdf2svg`, `pdfcrop` and `sed`. 

Note that I have built this on debian unstable and hence I haven't tested on anything else. Generally, though, if you have a full `texlive` distribution and GNU `bash` and `sed`, things should compile. Depending on your system you may need to adapt the method to produce `.svg` files from the produce `.pdf`.

## Current Examples (Updated Regularly...)

### Organic and Drug-Like Molecules

(Simple) organic molecules are usually the easiest to produce as they can be drawn mostly using multiples of the base angle. Each example is generally included as it includes something new, like the inclusion of charges, lone pairs, shifted double bonds, stereochemistry, psuedotransparency, etc.

1.  Aripiprazole -- a simple example showcasing the basics, how to colour atoms, how to construct lone and joined rings and the use of the base angle increment

    ![](svg/light/01.svg#gh-light-mode-only)

    ![](svg/dark/01.svg#gh-dark-mode-only)

2.  Venlafaxine showing the phenethylamine backbone -- shows how to construct rings using hooks and custom angles, rather than the normal ring syntax, which is done to construct a cyclohexane ring in the chair conformation. Also includes the use of the psuedotransparent colours for both atoms and bonds

    ![](svg/light/02.svg#gh-light-mode-only)

    ![](svg/dark/02.svg#gh-dark-mode-only)

3.  Escitalopram -- shows how to place a stereochemistry marker at a stereocentre as well as introducing the use of triple bonds

    ![](svg/light/03.svg#gh-light-mode-only)

    ![](svg/dark/03.svg#gh-dark-mode-only)

4.  Memantine -- shows the use of multiple hooks to create complex multicyclic/cage-like/diamondoid structures as well as how to place a lone pair

    ![](svg/light/06.svg#gh-light-mode-only)

    ![](svg/dark/06.svg#gh-dark-mode-only)

5.  Quetiapine -- shows how to rotate a part of the molecule by a custom angle, done so the 7 membered ring takes the preferred orientation

    ![](svg/light/09.svg#gh-light-mode-only)

    ![](svg/dark/09.svg#gh-dark-mode-only)

6.  Scopolamine -- another example of creating a multicyclic ring structure using hooks

    ![](svg/light/10.svg#gh-light-mode-only)

    ![](svg/dark/10.svg#gh-dark-mode-only)

7.  8-Chlorotheophylline -- just a typical caffeine-like molecule for fun and because I'd made it for a separate prohject :)

    ![](svg/light/11.svg#gh-light-mode-only)

    ![](svg/dark/11.svg#gh-dark-mode-only)

8.  Myristicin -- shows how to shift a double bond so that it is above/below a main chain for a cleaner look

    ![](svg/light/12.svg#gh-light-mode-only)

    ![](svg/dark/12.svg#gh-dark-mode-only)

9.  Benzydamine -- shows the use of relative angles (i.e. defined relative to the angle of the previous bond) which allows the side chains to have the angles they do

    ![](svg/light/13.svg#gh-light-mode-only)

    ![](svg/dark/13.svg#gh-dark-mode-only)

10. Coronene/Superbenzene -- a more complicated multi-ring example

    ![](svg/light/14.svg#gh-light-mode-only)

    ![](svg/dark/14.svg#gh-dark-mode-only)

11. Maitotoxin -- I included this both to challenge me and to show that even complicated molecules can be created with a relatively simple (if a bit long) process following the molecule from one end to another and adding side chains (it wasn't as bad as it looks, I promise!)

    ![](svg/light/17.svg#gh-light-mode-only)

    ![](svg/dark/17.svg#gh-dark-mode-only)

### Polymers

1.  Homopolymer polystyrene -- shows the addition of polymer brackets to indicate a repeating unit

    ![](svg/light/08.svg#gh-light-mode-only)

    ![](svg/dark/08.svg#gh-dark-mode-only)

### Inorganic Compounds

1.  Ferrocene derivative -- shows the use of invisible bonds used for alignment and creating nodes that can be used to add information -- in this case the ellipses on the rings

    ![](svg/light/05.svg#gh-light-mode-only)

    ![](svg/dark/05.svg#gh-dark-mode-only)

2.  Ir(ppy)3 -- shows how invisible bonds can be used to create big structures and keep their alignment relatively simply without doing a lot of annoying hooks or math

    ![](svg/light/07.svg#gh-light-mode-only)

    ![](svg/dark/07.svg#gh-dark-mode-only)

### Reaction Mechanisms

1.  Cycloaddition reaction (tetradehydro Diels-Alder (TDDA)) -- reinforces the use of invisible bonds as a means to keep alignment between separate fragments and place nodes for drawing; also shows the use of arrows, reaction conditions and how to align molecules relative to some feature; shows the use of mechanistic arrows with custom contours

    ![](svg/light/04.svg#gh-light-mode-only)

    ![](svg/dark/04.svg#gh-dark-mode-only)

2.  Decarboxylation of cyclic peroxyester to excited ketone -- shows how to place information adjacent to brackets surrounding a whole molecule using the same tools used to draw mechanistic arrows

    ![](svg/light/15.svg#gh-light-mode-only)

    ![](svg/dark/15.svg#gh-dark-mode-only)

3.  Nucleophilic aromatic substitution reaction -- shows the use of invisible arrows to space reactants out, as well as demonstrating that mechanistic arrows can be drawn between separate molecules, shows the placement of circled charges, shows that once you have one set of mechanistic arrows drawn, it's just a matter of copy/pasting and tweaking the controls and nodes

    ![](svg/light/16.svg#gh-light-mode-only)

    ![](svg/dark/16.svg#gh-dark-mode-only)
