# Jeremy Betz’s personal site

Source for [jeremybetz.github.io](https://jeremybetz.github.io), a lightweight personal site about data science, quantitative research, and soccer analytics.

The site is built with Jekyll and published through GitHub Pages. It deliberately keeps the original small static-site structure: pages and posts are written in Markdown or HTML, layouts use Liquid, and styles are maintained in Sass.

## Editing the site

- `index.html` is the home page.
- `about.md`, `projects.md`, and `archive.md` are the main site pages.
- `_posts/` contains earlier writing preserved as an archive.
- `_config.yml` contains site metadata, URLs, and GitHub Pages plugin configuration.
- `_layouts/`, `_includes/`, `style.scss`, and `_sass/` contain the shared presentation layer.

Keep current work concise and evidence-based. Historical posts should remain available unless there is a specific reason to remove them.

## Local preview

This repository intentionally does not include a Gemfile or lockfile. With Ruby and the GitHub Pages gem available locally, serve the site with:

```sh
gem install github-pages
jekyll serve
```

Then visit <http://127.0.0.1:4000>. Installing the gem is optional; GitHub Pages builds the site after changes are pushed to the deployment branch.

## Deployment

The published site is built by GitHub Pages from the `master` branch. Changes should be reviewed on a working branch, then merged or fast-forwarded into `master`; pushing `master` triggers the existing deployment process.
