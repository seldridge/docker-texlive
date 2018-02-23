# Docker image for texlive [![TexLive:2017](https://img.shields.io/badge/TeX%20Live-2017-blue.svg)](https://www.tug.org/texlive/acquire.html) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![download-size number-of-layers](https://images.microbadger.com/badges/image/seldridge/docker-texlive.svg)](https://microbadger.com/images/seldridge/docker-texlive)

This is based on [sumdoc/texlive-2017](https://hub.docker.com/r/sumdoc/texlive-2017/), with the addition of following programs:

- [latexmk](https://www.ctan.org/pkg/latexmk/)
- Python 2.7, pip, pyparsing, python-docx
- Python 3.6, scipy, numpy, matplotlib
- Java headless
- [pax](http://ctan.org/pkg/pax)
- [pdftk](https://www.pdflabs.com/tools/pdftk-the-pdf-toolkit/)
- Ghostscript
- Inkscape
- Pandoc
- Graphviz

Usage:

    docker run --rm -it -v $(pwd):/home seldridge/docker-texlive latexmk document.tex
