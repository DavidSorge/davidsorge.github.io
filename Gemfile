# frozen_string_literal: true

source "https://rubygems.org"

git_source(:github) {|repo_name| "https://github.com/#{repo_name}" }

# Core Jekyll - use version compatible with GitHub Actions
gem "jekyll", "~> 4.3.0"

# Required gems for modern Jekyll
gem "webrick", "~> 1.7"
gem "logger", "~> 1.4"

# Plugins required by the Index theme and our configuration
gem "jekyll-paginate", "~> 1.1"
gem "jekyll-sitemap", "~> 1.4"

# Additional gems that GitHub Actions might need
gem "rouge", "~> 4.0"
gem "kramdown-parser-gfm", "~> 1.1"

# Windows and JRuby specific gems
platforms :windows, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Windows file watching for better performance
gem 'wdm', '>= 0.1.0' if Gem.win_platform?
