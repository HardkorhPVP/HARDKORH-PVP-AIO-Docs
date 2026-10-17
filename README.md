# HARDKORH PVP AIO - documentation site

Public product documentation for **HARDKORH PVP AIO v1.0.0** (Feral Druid PvP, World of Warcraft: Midnight, Project Sylvanas),
by HardkorhPVP. This repository holds documentation only: no plugin source, no logs, no private material.

Built with [Jekyll](https://jekyllrb.com/) and the [Minimal Mistakes](https://mademistakes.com/work/jekyll-themes/minimal-mistakes/)
theme, used as a GitHub Pages remote theme (`mmistakes/minimal-mistakes@4.28.1`). No theme source is copied into this repository;
the local customizations are `assets/css/main.scss`, `_includes/hk-figure.html` and the theme's two hook includes
`_includes/head/custom.html` (favicons) and `_includes/footer/custom.html` (artwork credit).

## Structure

| Path | Content |
| --- | --- |
| `index.md` | Home page (splash layout) |
| `_pages/` | Documentation pages: Getting Started, HARDKORH, Feral Druid, Support |
| `_data/navigation.yml` | Masthead and sidebar navigation |
| `assets/css/main.scss` | HARDKORH palette and components on top of the Minimal Mistakes dark skin |
| `assets/images/brand/` | Wordmark, Marketplace banner and detail art |
| `assets/images/art/` | Decorative illustrations: home hero, arena artwork and per-page header crops (`headers/`) |
| `assets/images/favicons/` | Favicon and app icons; `site.webmanifest` is the web app manifest |
| `assets/images/screenshots/` | Privacy-sanitized in-game screenshots |
| `HEADER_VISUAL_MANIFEST.md` | Developer record of every page header composition (not published) |

## Local preview

Requires Ruby with Bundler (on Windows, RubyInstaller "Ruby+Devkit"):

```
bundle install
bundle exec jekyll serve
```

Then open the local server address Jekyll prints in the terminal; it ends in `/HARDKORH-PVP-AIO-Docs/`. The first build downloads
the remote theme and takes a minute or two.

## Publishing

GitHub Pages builds the site from the `main` branch (root folder) of `HardkorhPVP/HARDKORH-PVP-AIO-Docs`, as the project site
`https://hardkorhpvp.github.io/HARDKORH-PVP-AIO-Docs/`. `url` and `baseurl` in `_config.yml` match that address; every internal
link uses `relative_url`.
