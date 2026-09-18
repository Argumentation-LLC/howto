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

In the repository's **Settings → Pages → Build and deployment**, set **Source** to **GitHub Actions**. This site requires the bundled Jekyll build in `.github/workflows/pages.yml`, which installs the `just-the-docs` theme from the Gemfile. The built-in **Deploy from a branch** builder uses the `github-pages` gem and cannot build this configuration.

Review the changes in a separate branch or pull request. When the approved files are merged or pushed to `main`, the included GitHub Pages workflow builds and deploys the site. Check the workflow result after publication.

After correcting the publishing source, you can deploy the current `main` branch from **Actions → Deploy Jekyll site to Pages → Run workflow**. Re-running a failed **pages build and deployment** run will use the old built-in builder instead.

Several older Markdown filenames are retained intentionally so existing public documentation URLs continue to work.
