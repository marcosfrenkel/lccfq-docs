# LCCFQ-QHPC Documentation Page

This repository contains the documentation site for the LCCFQ project. 
It is composed of all the repositories hosted under the LLCF-QHPC GitHub organization.

## Getting Started

To build the documentation site locally, you need to have Python and a python package manager installed. We recommend using us `uv` since that is the package manager this project utilizes, but any will work. If you don't have `uv` installed, please see the [uv installation guide](https://docs.astral.sh/uv/getting-started/installation/)

To build and host the documentation locally and see live changes as you edit, run the following command:

```bash
uv run mkdocs serve
```

That command will start a webserver that host the documentation page at `http://127.0.0.1:8000`. 


## Basic Structure

The documentation site is built using [MkDocs](https://www.mkdocs.org/) and the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) theme. For a deeper explanation on how to use MkDocs, please see the [MkDocs documentation](https://www.mkdocs.org/user-guide/) or [MkDocs Material documentation](https://squidfunk.github.io/mkdocs-material/). The following is a quick overview of how to add content.

### Adding a New Category

To add a new category of documentation, you need to create a new directory inside of `docs` and add a new item in the `nav:` section of `mkdocs.yml`.

### Adding a New Page

To add a new page, you need to create a new markdown file inside of the folder whose category this page will live under. Once the file is created, add that page as a sublist of the section in the `nav` section of `mkdocs.yml`

