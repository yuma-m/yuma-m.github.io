# yuma.cloud

Source of <https://yuma.cloud/>, built with [Hugo](https://gohugo.io/).

## Requirements

- Hugo extended 0.169.0
- Dart Sass 1.107.1

Keep these versions in sync with `.github/workflows/gh-pages.yml`.

```sh
brew install hugo sass/sass/sass
```

## Setup

The theme is a fork of anatole ([yuma-m/anatole](https://github.com/yuma-m/anatole)) included as a git submodule.

```sh
git clone --recurse-submodules git@github.com:yuma-m/yuma-m.github.io.git
# or, in an existing clone
git submodule update --init
```

Theme changes (templates, SCSS, Font Awesome) go to the fork first; then commit the updated submodule pointer here. Site-specific overrides live in `layouts/`.

## Development

```sh
hugo server -D
```

## Deployment

Pushing to `main` runs `.github/workflows/gh-pages.yml`, which builds the site and deploys it to GitHub Pages (source: GitHub Actions), served at `yuma.cloud`. Pull requests run the build only.

This repository is public, so drafts and branches pushed here are visible to anyone. Keep unpublished writing local.

Sub-sites under the same domain (`rust-training/`, `moq-training/`, `moqros/`) are deployed from their own repositories and are listed in `extraSitemapPaths` in `hugo.toml`.
