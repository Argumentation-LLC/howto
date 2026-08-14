# Argumentation.io How-To Documentation

This repository contains the public documentation for [Argumentation.io](https://argumentation.io). It is a Jekyll site using the [Just the Docs](https://just-the-docs.github.io/just-the-docs/) theme and is deployed through GitHub Pages.

## Preview locally

With Ruby and Bundler installed:

```shell
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000`. The generated site is stored in `_site`.

## Publish

Review the changes in a separate branch or pull request. When the approved files are merged or pushed to `main`, the included GitHub Pages workflow builds and deploys the site. Check the workflow result after publication.

Several older Markdown filenames are retained intentionally so existing public documentation URLs continue to work.
