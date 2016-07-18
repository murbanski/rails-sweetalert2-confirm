source "https://rubygems.org"

# Declare your gem's dependencies in sweet_rails_confirm.gemspec.
# Bundler will treat runtime dependencies like base dependencies, and
# development dependencies will be added by default to the :development group.
gemspec

# Declare any dependencies that are still in development here instead of in
# your gemspec. These might include edge Rails or gems from your path or
# Git. Remember to move these dependencies to your gemspec before releasing
# your gem to rubygems.org.

# To use debugger
# gem 'debugger'

rails_version = ENV["RAILS_VERSION"] || "default"

rails = case rails_version
        when "master"
          {github: "rails/rails"}
        when "default"
          ">= 4.1.0"
        else
          "~> #{rails_version}"
        end

gem "rails", rails
gem "turbolinks"

source 'https://rails-assets.org' do
  gem 'rails-assets-sweetalert2'
end

group :development, :test do
  gem "jquery-rails"
  gem "test-unit"
  gem 'sass-rails'
  gem "capybara"
  gem "poltergeist"
  gem "rake"
end
