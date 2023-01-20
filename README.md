# Curriculum Vitae

[![compile-pdf](https://github.com/hfmark/cv/workflows/compile-pdf/badge.svg?event=push)](https://github.com/hfmark/cv/actions)

These are the Latex sources for my academic CV, based on a template by Leonardo Uieda.

**Download** the latest compiled PDF:
[hfmark_cv.pdf](https://hfmark.github.io/cv/hfmark_cv.pdf)

## Template

This template was created by [Leonardo Uieda](https://github.com/leouieda). You're free to reuse and modify this template under the terms of the BSD 3-clause License (see `LICENSE.txt`). 

To use it:

* Click on the ["Use this template"](https://github.com/leouieda/cv/generate)
  button to grab a copy of the repository.
* Make sure that you either copy all branches, or create a branch named `gh_pages` in your copy
  of the repository.
* In the settings for your copy of the repository, go to Actions -> Workflow Permissions, and 
  select 'Read and write permissions' and 'Allow Gihub Actions to create and approve pull requests'
  to enable the action that compiles and serves a pdf of your cv.
* Rename `hfmark_cv.tex`.
* Fill out the variables and fields in the `.tex` file.
* If you want to check your pdf before building it online (highly recommended!), install Tectonic 
  on your local machine, either from their website or using the conda
  `environment.yml` file provided in the repository.
* Compile the PDF locally to check the results with `make show`.
* Push your changes and GitHub Actions should do it's magic and serve the PDF
  at `https://YOURUSERNAME.github.io/cv/YOURNAME_cv.pdf`.

## Building

I use [Tectonic](https://tectonic-typesetting.github.io) to build the PDF from
the sources.
It's very convenient, can be installed from
[conda-forge](https://github.com/conda-forge/tectonic-feedstock),
and is faster than using a normal LaTeX compiler.
There are many ways to install it (see their website for instructions).

I highly recommend using the `Makefile`:

* `make`: builds the PDF
* `make clean`: removes the built PDF and any other generated files

## Deploying

A PDF is compiled automatically by GitHub Actions with every commit to the
`main` branch and uploaded to the `gh-pages` branch.
This way, the compiled PDF is updated and served automatically.

## License

All LaTeX template source code is distributed under the
[BSD 3-clause License](https://opensource.org/licenses/BSD-3-Clause).
