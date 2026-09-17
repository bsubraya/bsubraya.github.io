source "https://rubygems.org"

# ─────────────────────────────────────────────────────────────
#  This file is ONLY for previewing the site on your own laptop.
#  GitHub Pages builds the live site with its own pinned versions
#  and ignores this file entirely — so nothing here can break the
#  published site.
#
#  Usage:
#    bundle install                    (once, and after editing this file)
#    bundle exec jekyll serve --livereload
# ─────────────────────────────────────────────────────────────

gem "jekyll", "~> 4.3"

group :jekyll_plugins do
  gem "jekyll-feed",          "~> 0.17"
  gem "jekyll-sitemap",       "~> 1.4"
  gem "jekyll-redirect-from", "~> 0.16"
end

# Ruby 3.0+ no longer bundles the web server Jekyll uses to serve locally.
gem "webrick", "~> 1.8"

# Ruby 3.4 moved these out of the standard library. Listing them keeps
# `bundle install` quiet on newer Ruby versions.
gem "base64"
gem "bigdecimal"
gem "csv"
gem "logger"
gem "ostruct"
