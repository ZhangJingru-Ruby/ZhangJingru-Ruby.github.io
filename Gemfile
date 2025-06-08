# -- Gemfile --------------------------------------------------------------
# Minimal, un-pinned Jekyll stack that works on GitHub Actions AND Windows.
# Add extra plugins inside the :jekyll_plugins group when you need them.
# ------------------------------------------------------------------------
source "https://rubygems.org"

ruby ">= 3.2", "< 3.5"          # any ≥ 3.1 works; this is stable & supported
gem   "jekyll", "~> 4.3"

group :jekyll_plugins do
  gem "jekyll-feed"       # RSS
  gem "jekyll-seo-tag"    # SEO <title>/<meta>
  gem "jekyll-sitemap"    # /sitemap.xml
  gem "jekyll-tagging"    # tag pages + tag clouds  ← **the one GitHub-Pages blocks**
end

# Local-only helpers (ignored on Linux runner)
gem "webrick", ">= 1.7", platforms: [:mingw, :x64_mingw, :mswin]
gem "tzinfo-data",        platforms: [:mingw, :x64_mingw, :mswin]
