# jerushatwinklefrancis.github.io

## Overview

This repository contains my personal website created using Quarto for DSCI 521 Milestone 3. The website includes personal pages together with blog posts demonstrating computational analyses in both Python and R.

## Prerequisites

Install the following software before building the website:

- Git
- Quarto
- Python 3.14
- uv
- R (version 4.6.1 or compatible)

The project uses `renv` to manage the R environment.

## Build Instructions

Run the following commands from a terminal in the root directory of the repository.

Clone the repository:

```bash
git clone https://github.com/jerushatwinklefrancis/jerushatwinklefrancis.github.io.git
cd jerushatwinklefrancis.github.io
```

### Restore the Python environment

```bash
uv sync
```

### Restore the R environment

Open R in the project directory and run:

```r
renv::restore()
```

### Render the website

```bash
uv run quarto render
```

The rendered website will be created in the `docs/` directory.

## Data Sources

- **Python post:** Palmer Penguins dataset by Allison Horst: https://allisonhorst.github.io/palmerpenguins/
- **R post:** The built-in `mtcars` dataset included with R.

The rendered website is written to the `docs/` directory, which is configured for GitHub Pages. After rendering, the website can be viewed locally by opening `docs/index.html` or published through GitHub Pages.