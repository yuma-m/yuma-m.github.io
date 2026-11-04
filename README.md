# yuma.cloud

Source of <https://yuma.cloud/>, built with [Hugo](https://gohugo.io/).

## Requirements

- Hugo extended 0.169.0
- Dart Sass 1.107.1

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

## Development

```sh
hugo server -D
```

## Deployment

Pushing to `main` runs `.github/workflows/gh-pages.yml`, which builds the site and deploys it to GitHub Pages (source: GitHub Actions), served at `yuma.cloud`. Pull requests run the build only.
