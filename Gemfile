# frozen_string_literal: true

source "https://rubygems.org"

git_source(:github) {|repo_name| "https://github.com/#{repo_name}" }

# Core Jekyll
gem "jekyll", "~> 4.2"

# Future compatibility - add logger gem for Ruby 3.5+ compatibility
gem "logger"

# Plugins required by the Index theme and our configuration
gem "jekyll-paginate"
gem "jekyll-sitemap"

# Windows and JRuby specific gems
platforms :windows, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Windows file watching for better performance
gem 'wdm', '>= 0.1.0' if Gem.win_platform?
