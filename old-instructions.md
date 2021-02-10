# Primer Template

A template for a simple GitHub pages website using the Primer theme.

# Demo

See what this looks like at [pavopax.github.io/primer-template/](https://pavopax.github.io/primer-template/)

# Get started

1) Create content:

  * Create a new repository on github.com
  * Add a README.md file with some content into the repository

2) Publish so others can see it:

  * Go to repository `Settings` (tab on top right) - scroll down to `GitHub
    Pages` and in `Source` select `master branch`
  * The page will refresh. Scroll down again to `GitHub Pages` and find the
    link to your GitHub Page under "Your site is published at ..".
  * Open the link to view your website
  * You can now share that link!

That's it!

# Update content

  * For a single page, README.md works fine.
  * For multiple pages, consider renaming `README.md` to `index.md`

For a more robust template, you can clone this repository as a starting point,
see "Extensions".

# Update exiting website

*If you only want to add local preview to an existing website, see below for ["Add
local preview to any Github Pages website"](#add-local-preview-to-any-github-pages-website).*

# Extensions

With this website template, you will be able to **preview your changes
locally** before deploying to GitHub Pages.

1. Clone or fork this repository.
1. On command line or Terminal, `cd /docs`.
1. Run `bundle exec jekyll serve` to preview the site (open the url in
   browser).
    * If you can't run `bundle`, etc, then you may need to install a few
      things, see below.

Now, customize and/or deploy as below.

# Install

For local preview (`bundle` command), you need `jekyll`:

1. Install a full [Ruby development
   environment](https://jekyllrb.com/docs/installation/)
1. Install Jekyll and [bundler](https://jekyllrb.com/docs/ruby-101/#bundler)
   [gems](https://jekyllrb.com/docs/ruby-101/#gems)

		gem install jekyll bundler

Reference: [jekyllrb.com/docs/](https://jekyllrb.com/docs/).

# Customize

### Theme

Don't like the theme? You can use any Jekyll/Github Pages theme. [Learn more](https://help.github.com/en/articles/adding-a-jekyll-theme-to-your-github-pages-site).


### Content

Edit content in `/docs`. Start with `index.md`, which is your main landing
page.

Then, edit (or delete) the following:

1. `_includes/header.html`
1. `_includes/footer.html`

If you delete either of these, also remove relevant lines ~12-14 in
`_layouts/default.html`.

# Deploy

1. Push your code to your GitHub space
1. Go to repository `Settings` - scroll down to `GitHub Pages` and in `Source`
   select `master branch /docs` folder and then `Save`.
1. The page will refresh. Scroll down again to `GitHub Pages` and find the link
   to your GitHub Page under "Your site is ready to be published at".

# Details

This page is served on GitHub from `/docs` so that you can easily include your
website along with your project code, all in the same repo.

# Enhancements

* [ ] add blog posts (just email me if you want this, see bottom)


This template includes minor edits from the [default theme for GitHub Pages,
the Primer theme](https://github.com/pages-themes/primer). The changes are in
`/docs/_layouts/default.html`, as follows:

  * removed the first linked header 
  * add header/footer with content from `/_includes`

# Add local preview to any Github Pages website

If you already have a GitHub Pages website, you can preview it locally.

[In `/docs`] create `Gemfile` containing:

	gem "github-pages", group: :jekyll_plugins

Then, run `bundle exec jekyll serve` and open the URL printed in the
message. Install `bundle` as described above in [Install](#install).

### Notes

The absolute bare-bones set-up actually needs only one file:

1. Create `index.md` in some directory
1. Run `jekyll serve` to preview it

(provided you have jekyll installed.

However, the above will not style your page with the Github Pages theme. Plus,
`jekyll` recommends using `bundle` for package version control.

# References

Primer: Customize the [Default Github Pages theme](https://github.com/pages-themes/primer)

Error "No repo name found" "Site could not be built" requires editing default
template. See
[stackoverflow.com/a/48832099/3217870](https://stackoverflow.com/a/48832099/3217870).
