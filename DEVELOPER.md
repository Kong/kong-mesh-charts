# Developer documentation

Welcome to the developer documentation for Kong Mesh Helm chart GH page! Below is some
helpful information to walk you through customization and other features involving
the GitHub page theme for this site.

## Editing styles

All custom styles are located in `assets/css/style.scss`. This structure is important
and must stay intact in order for the styles to be recognized and processed by Jekyll.

[Primer](https://github.com/pages-themes/primer) is the GitHub Pages Jekyll theme
that is used as a base.

## Page content

All page content is located in `README.md`. Please note that the logo image is
placed at the top so that it acts as a page header, with the `h1` title below it
to act as the main page title.

## Running locally

This repo contains a `Gemfile` that is required to run Jekyll and contains the
needed dependencies. Ruby 2.1.0 or higher is required. If you don't already have it,
you can [download it here](https://www.ruby-lang.org/en/downloads/).

1. Run `bundle install` to install the dependencies for running Jekyll locally
2. Run `bundle exec jekyll serve` to run the site
3. View the site in your browser at `http://localhost:4000`

Any changes you make will be automatically compiled.

**Note:** There is no hot-reloading in the browser with this approach.
When your changes are made, make sure to refresh your browser to see the updates.

If you would like to read more about running this site locally, please refer to
the [GitHub Pages documentation](https://docs.github.com/en/enterprise/2.14/user/articles/setting-up-your-github-pages-site-locally-with-jekyll).

## Customization

For deeper customization, please refer to 
[Jekyll's configuration options](https://jekyllrb.com/docs/configuration/options/).
This site currently only uses the `exclude` feature, which is located in `_config.yaml`.
