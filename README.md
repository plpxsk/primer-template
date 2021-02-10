# Primer Template

A template for a simple GitHub pages website using the Primer theme.

# Demo

See what this looks like at [pavopax.github.io/primer-template/](https://pavopax.github.io/primer-template/)

# Get started

Create the simplest GitHub pages site possible:

1) Create content:

  * Create a new repository on GitHub (GitHub Enterprise is ok)
  * Add a README.md file with some content into the repository

2) Publish so others can see it:

  * Go to repository `Settings` (tab on top right) - scroll down to `GitHub
    Pages` and in `Source` select `master branch`
  * The page will refresh. Scroll down again to `GitHub Pages` and find the
    link to your GitHub Page under "Your site is published at ...".
  * Open & share link


# Update content

  * For a single page, README.md works fine.
  * For multiple pages, consider renaming `README.md` to `index.md`

For a more robust template, you can clone this repository as a starting point,
see "Extensions".


# Customize

To remove the Header link, create `_config.yml` and add:

```
name: My Website
title: null
```

Both are required. Learn more about this at [pages-themes/primer#40](https://github.com/pages-themes/primer/issues/40)

# Preview

> You can build your GitHub Pages site locally to preview and test changes to your site.

See official [Github Docs](https://docs.github.com/en/github/working-with-github-pages/testing-your-github-pages-site-locally-with-jekyll).
