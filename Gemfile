# frozen_string_literal: true

source "https://rubygems.org"

## From bjt gemspec file, not sure if need to 
    # include each gem explicitly

# spec.add_runtime_dependency "jekyll", "~> 3.9.3"
# spec.add_runtime_dependency "jekyll-paginate", "~> 1.1"
# spec.add_runtime_dependency "jekyll-sitemap", "~> 1.4"
# spec.add_runtime_dependency "kramdown-parser-gfm", "~> 1.1"
# spec.add_runtime_dependency "kramdown", "~> 2.3.2"
# spec.add_runtime_dependency "webrick", "~> 1.8"

# spec.add_development_dependency "bundler", ">= 1.16"
# spec.add_development_dependency "rake", "~> 12.0"


####################
# From site v1

gem "github-pages", group: :jekyll_plugins
gem "jekyll-include-cache", group: :jekyll_plugins
gem "jekyll-remote-theme"

# If you have any plugins, put them here!
group :jekyll_plugins do
  gem "jekyll-paginate"
  gem 'jekyll-sitemap'
  gem "jekyll-gist"
#   gem "jekyll-feed", "~> 0.12"
#   gem "jekyll-algolia"
#   gem 'jekyll-seo-tag'
#   gem "beautiful-jekyll-theme", "6.0.1"
#   gem "jemoji"
  gem "kramdown", "~> 2.3.2"
  gem "kramdown-parser-gfm", "~> 1.1"
  gem "webrick", "~> 1.8"
end


# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]

# Lock `http_parser.rb` gem to `v0.6.x` on JRuby builds since newer versions of the gem
# do not have a Java counterpart.
gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]
