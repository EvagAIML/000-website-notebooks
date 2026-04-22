# 000-website-notebooks
This repository automatically publishes AI/ML case studies (Jupyter notebooks) to GitHub Pages.


## How it works
On every push to `main`, GitHub Actions:
- Converts each notebook in `/notebooks/**` into a static HTML page
- Publishes a homepage index listing all case studies
- Creates downloadable artifacts per case study:
  - notebook.html
  - notebook.ipynb
  - notebook.py (if present)
  - assets/ (if present)


## Repo structure
- `notebooks/<case-study-slug>/` contains your source notebooks
- `site/` is generated during Actions (do not edit manually)

Naming convention:
`what-problem__problem-type__model-family-or-study`
(lowercase, hyphens inside segments, double underscores between segments)

For instructions on updating or adding case studies, see `CONTRIBUTING.md`.


## Assets

Live Website: https://time-chuck-90820705.figma.site/

Live Links: https://evagaiml.github.io/000-website-notebooks/



<!-- trigger build -->
