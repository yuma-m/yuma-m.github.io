# CLAUDE.md

Personal site at <https://yuma.cloud/>, built with Hugo. See `README.md` for setup and commands.

## Rules

- Keep the Hugo and Dart Sass versions in `README.md` in sync with `.github/workflows/gh-pages.yml`.
- The theme is a fork (`themes/anatole` -> `yuma-m/anatole`). Make theme changes (templates, SCSS, Font Awesome) in the fork first, then commit the updated submodule pointer here. Put site-specific overrides in `layouts/` instead of editing the theme.
- This repository is public: drafts and branches pushed here are visible to anyone. Keep unpublished writing local.
- `rust-training/`, `moq-training/` and `moqros/` under the same domain are deployed from their own repositories. They are listed in `extraSitemapPaths` in `hugo.toml`; don't add content for them here.
