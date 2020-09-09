# About 3DC

![ci](https://github.com/3DCdsc/About/workflows/ci/badge.svg?branch=master)

### Add / Edit Pages

All pages are written in MarkDown (`.md`) located under the directory `docs/` on Master branch.


### This repo is using MkDocs with a material theme

```
pip install mkdocs-material
```

### About MkDocs

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

### MkDocs Commands on local

* `mkdocs new [dir-name]` - Create a new project. (You don't need to use this for existing project)
* `mkdocs serve` - Start the live-reloading docs server. (You can use this to preview your changes at local)
* `mkdocs build` - Build the documentation site. (You don't need to do this, this repo's CI will build on push and update the GitHub Page)
* `mkdocs -h` - Print help message and exit.

### Project layout
```
    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.
```
