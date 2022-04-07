# Primer Template

A template for a simple GitHub pages website using the Primer theme.

# Demo

See what this looks like at [plpxsk.github.io/primer-template/](https://plpxsk.github.io/primer-template/)

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

# Snippets

## Images & Paths

Insert image into markdown, and using jekyll relative paths (so that preview
works locally and when deployed):

```html
<img src="img/mittens_logo.jpg" alt="image" width="800">
<img src="{{ "/img/mittens_logo.jpg" | absolute_url }}" width="800">
```
## Blog post

Link to blog post from `_posts` (XYZ-blog-post-name doesn't need md nor html
extension):

	[text here]({{ site.baseurl }}{% post_url 2018-06-01-blog-pose-name %})

## List all posts

```html
# Posts
{% for post in site.posts %}

## {{ post.title }}
<p>
    <i>{{ post.date | date: page.date |  date: '%B %d, %Y' }}</i><br>
    <i>{{ post.author }}</i>
</p>

{{post.excerpt}}

<a href="{{ post.url | absolute_url }}">Read the article ></a>

<br>

{% endfor %}
```

## List all posts for given tag

```html
{% for tag in site.tags %}
<!-- tag is a tuple: (tag_name, [posts]) -->
{% if tag[0] == "science" %} <!-- science is the tag -->
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url | absolute_url}}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endif %}
{% endfor %}
```

## List all tags

```html
<p>
{% for tag in site.tags %}
	{{ tag[0] }}
{% endfor %}
</p>
```
