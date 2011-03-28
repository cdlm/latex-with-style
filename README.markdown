# What's this?

A few pieces of advice for LaTeX users, to help them prepare documents with better typography, streamline their writing workflow, and write maintainable LaTeX code.

### Compiling

Just pass `main.tex` through the usual PDFLaTeX process, or adopt the lazy way:

    latexmk -pdf main

The document uses the [`tufte-latex` class][tufte-google], which is [bundled with the major TeX distributions][tufte-ctan]. You might want to check for an up-to-date version though, since I'm updating [TeXlive][] with obsessive-compulsive frequency :)


# Included packages

I'm trying to keep the reuseable parts of the setup code modularized out of the main file into proper packages. At one point, these might be maintained separately, but they will live here for a while.


### LaTeX logo for the Lato font

The LaTeX logo was not looking very nice when set in [Lato][] with the original definition; `lato-latex.sty` redefines `\TeX` and `\LaTeX` to better fit. The code was inspired by [`arsclassica.sty`][arsclassica].


### Tweaks for to-do notes

I use [`todonotes.sty`][todo] while writing and it needed a few tweaks to fit `tufte-latex`; this is in `todo-setup.sty`.


[tufte-google]: http://code.google.com/p/tufte-latex/ "A Tufte-inspired LaTeX class for producing handouts, papers, and books"
[tufte-ctan]: http://ctan.tug.org/pkg/tufte-latex "tufte-latex on CTAN"
[texlive]: http://www.tug.org/texlive/
[lato]: http://www.fontsquirrel.com/fonts/lato "Lato, by Łukasz Dziedzic"
[arsclassica]: http://ctan.tug.org/pkg/arsclassica "An extension of classicthesis"
[classicthesis]: http://ctan.tug.org/pkg/classicthesis "A document class with a Bringhurst-inspired design"
[todo]: http://ctan.tug.org/pkg/todonotes


# License

This work by [Damien Pollet](http://people.untyped.org/damien.pollet) is licensed under a [Creative Commons Attribution-ShareAlike 3.0 License](http://creativecommons.org/licenses/by-sa/3.0/).
