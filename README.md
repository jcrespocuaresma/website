# Jesús Crespo Cuaresma — academic website

A deliberately slim academic website with four pages:

- Home
- Research
- Publications
- Teaching

The repository contains both **Quarto source files** (`*.qmd`) and a **ready-to-publish static version** in `docs/`.

## Publish immediately with GitHub Pages — no software required

1. Create a GitHub account if you do not already have one.
2. Create a new repository. A simple name is `academic-site`. If you name it `<YOUR-GITHUB-USERNAME>.github.io`, the site will live directly at `https://<YOUR-GITHUB-USERNAME>.github.io/`.
3. Upload the **contents of this folder** to the repository, including the `docs` folder. Keep the folder structure unchanged.
4. Open the repository on GitHub and go to **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select branch **main** and folder **/docs**, then click **Save**.
7. GitHub will publish the site. For a repository called `academic-site`, the address will normally be `https://<YOUR-GITHUB-USERNAME>.github.io/academic-site/`.

The files under `docs/` are already rendered, so you do not need Quarto for this first publication.

## Edit and preview with Quarto

For ongoing maintenance, install Quarto from https://quarto.org/ and edit the `.qmd` files in the root folder.

Preview locally:

```bash
quarto preview
```

Regenerate the `docs/` folder:

```bash
quarto render
```

Then commit/push both the source files and the updated `docs/` folder to GitHub.

## Add a PDF CV

The updated LaTeX source is in:

`files/CV_Crespo_Cuaresma_DOI_updated.tex`

When you have a current PDF, save it as:

`files/CV_Jesus_Crespo_Cuaresma.pdf`

and copy the same PDF to:

`docs/files/CV_Jesus_Crespo_Cuaresma.pdf`

You can then add a CV link to the homepage or navbar.

## Custom domain

After the GitHub Pages version is working, you can add a custom domain under **Settings → Pages → Custom domain**. Configure the corresponding DNS records with your domain provider. GitHub recommends verifying the domain for security.

## Main files to edit

- `_quarto.yml` — navigation and global site settings
- `index.qmd` — homepage
- `research.qmd` — research profile
- `publications.qmd` — selected and complete publication lists
- `teaching.qmd` — teaching
- `styles.css` — appearance

## Notes

- The design intentionally uses no photograph or stock imagery.
- The complete peer-reviewed publication list is collapsed by default to keep the site visually light.
- DOI links are clickable and use `https://doi.org/...`.
- External profile links currently point to WU Research, ORCID, the WU department page, the World Poverty Clock and the World Emissions Clock.
