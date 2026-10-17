# HARDKORH PVP AIO - documentation site

Public product documentation for **HARDKORH PVP AIO v1.0.0** (Feral Druid PvP, World of Warcraft: Midnight, Project Sylvanas),
by HardkorhPVP. This repository holds documentation only: no plugin source, no logs, no private material.

Built with [Jekyll](https://jekyllrb.com/) and the [Minimal Mistakes](https://mademistakes.com/work/jekyll-themes/minimal-mistakes/)
theme, used as a GitHub Pages remote theme (`mmistakes/minimal-mistakes@4.28.1`). No theme source is copied into this repository;
`assets/css/main.scss` and `_includes/hk-figure.html` are the only local customizations.

## Structure

| Path | Content |
| --- | --- |
| `index.md` | Home page (splash layout) |
| `_pages/` | Documentation pages: Getting Started, HARDKORH, Feral Druid, Support |
| `_data/navigation.yml` | Masthead and sidebar navigation |
| `assets/css/main.scss` | HARDKORH palette and components on top of the Minimal Mistakes dark skin |
| `assets/images/brand/` | Marketplace banner and detail art |
| `assets/images/screenshots/` | Privacy-sanitized in-game screenshots |

## Local preview

Requires Ruby with Bundler (on Windows, RubyInstaller "Ruby+Devkit"):

```
bundle install
bundle exec jekyll serve
```

Then open the local server address Jekyll prints in the terminal. The first build downloads the remote theme and takes a minute
or two.

## Publishing (not active yet)

The site is not published. When a GitHub repository and GitHub Pages are set up, the expected pattern for a project site is
`https://<owner>.github.io/<repository>/`. Set `url` and `baseurl` in `_config.yml` to match the address GitHub reports at that
time; every internal link uses `relative_url`, so no page needs to change.
