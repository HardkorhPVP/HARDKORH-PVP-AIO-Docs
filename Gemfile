source "https://rubygems.org"

# GitHub Pages build environment: the same Jekyll version and whitelisted plugins GitHub Pages uses.
gem "github-pages", "~> 232", group: :jekyll_plugins
# Required by the Minimal Mistakes remote theme.
gem "jekyll-include-cache", group: :jekyll_plugins

# Local preview on Ruby 3.x: WEBrick is no longer bundled with Ruby.
gem "webrick", "~> 1.8"

# Windows: time zone data for Jekyll.
platforms :windows do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end
