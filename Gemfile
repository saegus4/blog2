# frozen_string_literal: true
source "https://rubygems.org"

ruby "3.4.2"                         # pin to whatever you run locally
gem   "jekyll", "~> 4.4"
gem   "webrick", "~> 1.8"            # needed on Ruby ≥3

group :jekyll_plugins do
  gem "jekyll-theme-chirpy", "~> 5.4"
end

group :test do                       # only installed locally unless you say otherwise
  gem "html-proofer", "~> 5.0"
end

# Windows / JRuby helpers
install_if -> { RUBY_PLATFORM =~ /mingw|mswin|java/ } do
  gem "tzinfo", "~> 1.2"
  gem "tzinfo-data"
end
gem "wdm", "~> 0.1.1", install_if: Gem.win_platform?
