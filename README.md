# intro

Welcome to my blogging website.

[![Deploy to Github Pages](https://github.com/cham11ng/sagarchamling.com/actions/workflows/deploy.yml/badge.svg)](https://github.com/cham11ng/sagarchamling.com/actions/workflows/deploy.yml)
[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

## prerequisites

- Install Homebrew
- Install Bun
- Install Git
- Install Go
- Install Hugo - Make sure you install latest version of hugo(>=0.119.0).

### setup and run

```bash
$ make
setup                Setup site development mode.
upgrade              Upgrade bun packages.
clean                Clean old builds.
build                Build minified version of site.
pretty               Format site using prettier.
compress             Compress all .png files into .webp format.
sync                 Synchronize with the latest theme.
help                 Help using make file.

$ make setup

or

$ bun install # install npm packages for pre-commit hook and prettier

$ git submodule update --init --recursive # clone submodule
$ git submodule update --remote --merge # update theme

```

```bash
hugo serve
```

### adding folder

```bash
# Syntax
hugo new --kind folder blogs/<folder-name>/_index.md

# Example
hugo new --kind folder blogs/tech/_index.md
```

### adding blog

```bash
# Syntax
hugo new --kind blog blogs/<folder-name>/<blog-title>.md

# Example
hugo new --kind blog blogs/tech/how-i-setup-my-website.md
```

### adding slides

```bash
# Syntax
hugo new --kind slides slides/<blog-title>.md

# Example
hugo new --kind slides slides/github-essentials.md
```

### setup and run webp converter

```bash
brew install webp

make compress
```

## inspired from

Hugo [PaperMod](https://github.com/adityatelange/hugo-PaperMod/).

## license

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
