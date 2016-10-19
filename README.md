# Latex Thesis Template
Generate a thesis from a mindmap (`.mm` file).

I suggest using [Docear](http://www.docear.org/) to build such a mindmap. It features an integrated reference manager.
References on nodes are transformed to latex citations.

## Usage
Structuring the mindmap: see [documentation of mm2latex](mm2latex/README.md).

Add (e.g. link):
- `body.mm`: input mindmap file
- `bib.bib`: bibliography

Modify:
- `metadata.tex`: author name, date, thesis title etc.

Install (dependencies):
- `tex`: some Tex distribution, e.g. _Tex Live_
- `arara`: manages the pdflatex and biber build
- `xsltproc`: transforms the mindmap to Latex using an `xslt` file

Init submodules:
- `git submodule init`: Inits the `mm2latex` submodule

Build:
- `./build.sh`