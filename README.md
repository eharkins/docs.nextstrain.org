# docs.nextstrain.org

A prototype umbrella documentation project for Nextstrain, hosted at [docs.nextstrain.org](https://docs.nextstrain.org), using:

- [Read The Docs](https://readthedocs.org)
- [Sphinx](http://sphinx-doc.org)
- [Markdown](https://markdownguide.org) and [reStructuredText](https://docutils.sourceforge.io/rst.html) ([quick ref](https://docutils.sourceforge.io/docs/user/rst/quickref.html), [quicker ref](https://simonwillison.net/2018/Aug/25/restructuredtext/))
- [Subprojects](https://docs.readthedocs.io/en/stable/subprojects.html) for Augur and the CLI (plus maybe Auspice and other component/build-specific documentation in the future)
- Our custom [Sphinx theme](https://github.com/nextstrain/sphinx-theme) to provide consistent, branded styling.

## Building the docs

Build dependencies are managed with [Conda](https://conda.io).  Install them
into an isolated environment named `docs.nextstrain.org` with:

    conda env create

Enter the environment with:

    conda activate docs.nextstrain.org

You can now build the documentation with:

    make html

which invokes Sphinx to build static HTML pages in `build/html/`.  You can view
them by running:

    open build/html/index.html

Leave the environment with:

    conda deactivate
