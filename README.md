# Jesús Crespo Cuaresma — academic website

This is a deliberately slim three-section academic site inspired by the clean profile/content layout of jhelvy.com.

## Top navigation

- About
- Research
- Teaching

The profile column contains only: CV, WU page, ORCID, LinkedIn.

## Editing

Edit the Quarto source files:

- `index.qmd` — About
- `research.qmd` — Research and selected publications
- `teaching.qmd` — Teaching
- `styles.css` — appearance
- `_quarto.yml` — navigation/site configuration

The currently published static files are in `docs/`.

## Publishing on GitHub Pages

For repository `jcrespocuaresma/website`:

1. Upload/replace the files in the repository.
2. Keep GitHub Pages set to **Deploy from a branch**.
3. Branch: `main`.
4. Folder: `/docs`.

The live URL is:

https://jcrespocuaresma.github.io/website/

## Photo crop

The portrait is displayed with CSS using `object-fit: cover` and `object-position`. To adjust the crop, edit this rule in `styles.css`:

```css
.profile-photo {
  object-position: 50% 18%;
}
```

The first number moves the crop left/right; the second moves it up/down.
