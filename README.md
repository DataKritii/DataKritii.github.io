# DataKritii portfolio site

Source for **https://datakritii.github.io/**, published with GitHub Pages from the `master` branch.

## Files

```
index.html              The whole page: header, intro, projects, skills, about, contact
assets/style.css        Styles. Brand colours are defined once at the top (:root)
assets/images/          Logo, favicon and project screenshots
```

## Preview changes before publishing

Double-click `index.html` to open it in your browser. Refresh after each edit.

## Add a project

1. In `index.html`, find the comment **HOW TO ADD A PROJECT**.
2. Copy an entire `<article class="project"> ... </article>` block and paste it **above** the others.
   so the newest project comes first.
3. Change the title, description, results, tags and links. For the label above the title
   (`class="kind"`), use `Business intelligence` or `Data science`.
4. Save a screenshot in `assets/images/` and point the `<img src="...">` to it.
5. To feature it (wide card with the amber bar), use `class="project project-featured"`.
6. If the project was listed under **Next up**, delete that line.

## Add the Streamlit link

Find `data-live-link` in `index.html` and paste the app URL between the quotes in `href=""`.
While it's empty, the page shows "Live dashboard coming soon".

## Publish

```bash
git add .
git commit -m "Describe the change"
git push
```

The live site updates within a minute or two.
