# Contributing (Updating / Adding Case Studies)

## Update an existing case study
1) Go to: `notebooks/<case-study-slug>/`
2) Replace the file(s):
   - `<slug>.ipynb`
   - `<slug>.py` (optional but recommended)
3) Commit to `main`
4) GitHub Actions rebuilds and redeploys automatically.
   - URLs do not change.

## Add a new case study
1) Create folder: `notebooks/<new-slug>/`
2) Inside it, add:
   - `<new-slug>.ipynb`
   - `<new-slug>.py` (optional but recommended)
   - `assets/` (optional folder for images/files)
3) Commit to `main`
4) GitHub Actions publishes it and it appears on the homepage automatically.

## Assets
Put images/diagrams/files here:
`notebooks/<slug>/assets/`

Assets are copied to:
`/<slug>/assets/` on the published site.

## Do not
- Do not edit the `gh-pages` branch manually.
- Do not put notebooks in the repo root.
- Do not edit generated HTML by hand (it is overwritten on each build).

## Troubleshooting
Check:
Actions → Build Notebooks → open the failed step.

Most common issues:
- Folder slug and notebook base name do not match exactly
- Wrong capitalization
- Missing `.ipynb` in a case study folder
