# Drafts

Quarto skips folders that start with an underscore, so pages here are never published.

`Teaching.qmd` is the full Teaching page (built from the teaching statement), parked while it's being revised.
`Blog.qmd` is The Confluence placeholder page.

To publish either one: move it back to the main folder, uncomment its line in the navbar section of `_quarto.yml`, then run `quarto render` and push.
Its images (images/web/...) and styles (the "Teaching page" section of styles.css) are already on the site, so it will look the same when it returns.
