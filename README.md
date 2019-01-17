Zenburn color theme for LaTeX
=============================

A theme to bring the [Zenburn] color scheme into LaTeX.  This defines
the colors using `xcolor`, styles for use with `listings`, `tcolorbox`
environments for wrapping code snippets, and a `beamer` color theme.

Installation
------------

To install, run

    scons

and copy the `.sty` files to somewhere LaTeX can find them.  You will
need the [dtxtools] for `SCons`.

Alternatively, you can run

    pdflatex zenburn-latex.ins
    pdflatex zenburn-latex.dtx

(repeat as necessary to resolve the references) by hand.

Usage
-----

To use, simply add `\usepackage{zenburn}` or `\usetheme{zenburn}` to
your document.

[zenburn]: http://kippura.org/zenburnpage/
[dtxtools]: https://github.com/kprussing/scons-dtxtools
