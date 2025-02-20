# pdf

This directory contains the script and related resources to generate a PDF document with all the `tldr` pages.

## Highlights

- No LaTeX dependencies for generating the PDF.
- 3 available color-schemes: *Basic*, *Solarized Light* and *Solarized Dark*. More can be added easily through CSS.

## Requirements

The PDF is generated by first converting the Markdown files to HTML, and then rendering those HTML files as a PDF. It depends on the `markdown` and `weasyprint` libraries. To install the dependencies, run:

    python3 -m pip install -r requirements.txt

Make sure OS specific dependencies for WeasyPrint are installed by following the instructions [here](http://weasyprint.readthedocs.io/en/latest/install.html).

## Usage

Generating the PDF is as simple as running:

    python3 render.py <path-to-pages-directory> [--color <color-scheme>] [--output <filename>]

Complete information about the arguments can be viewed by running:

    python3 render.py --help

Available color schemes:

- `basic`
- `solarized-light`
- `solarized-dark`

## Preview

![cryptsetup in the Basic color-scheme.](https://user-images.githubusercontent.com/29029116/35637791-4e42af80-06db-11e8-8b8e-42ce6c905ff4.jpg)
![cryptsetup in the Solarized Light color-scheme.](https://user-images.githubusercontent.com/29029116/35637798-51e3784a-06db-11e8-9576-6e57ef5c5c20.jpg)
![cryptsetup in the Solarized Dark color-scheme.](https://user-images.githubusercontent.com/29029116/35637801-54449fce-06db-11e8-93f7-d90cdc34044b.jpg)
