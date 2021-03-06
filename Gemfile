# frozen_string_literal: true

source 'https://rubygems.org'

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?('/')
  "https://github.com/#{repo_name}.git"
end

ruby '2.4.1'
gem 'rails', '5.0.2'

# Servers
gem 'thin', '~> 1.7'

# Multi-environment configuration
gem 'simpleconfig', '~> 2.0'

# API
gem 'rabl', '~> 0.13.1'

# ODM and related
gem 'client_side_validations', '~> 9.3'
gem 'client_side_validations-simple_form', '~> 6.2'
gem 'kaminari', '~> 1.0'
gem 'kaminari-mongoid', '~> 1.0'
gem 'mongoid', '~> 6.1'
gem 'mongoid-slug', '~> 5.3'
gem 'mongoid_geospatial', '~> 3.1'
gem 'mongoid_paranoia', '~> 0.3'
gem 'validates_timeliness', '~> 4.0'
gem 'validates_timeliness-mongoid', github: 'johnnyshields/validates_timeliness-mongoid'

# Authentication framework
gem 'devise', '~> 4.2'

# Geospatial data library
gem 'rgeo', '~> 0.6.0'

# Facebook integration
gem 'koala', '~> 3.0'
gem 'omniauth-facebook', '~> 4.0'

# Performance and Exception management
gem 'airbrake', '~> 6.0'
gem 'newrelic_rpm', '~> 4.1'

# Security
gem 'secure_headers', '~> 3.6'

# Miscellanea
gem 'google-analytics-rails', '~> 1.1'
gem 'http_accept_language', '~> 2.1'
gem 'jquery-rails', '~> 4.3'
gem 'resque', '~> 1.27', require: 'resque/server' # Resque web interface
gem 'sinatra', '~> 2.0.0.rc2' # Needed by resque/server
gem 'slim-rails', '~> 3.1'

# Assets
gem 'autoprefixer-rails', '~> 6.7'
gem 'coffee-rails', '~> 4.2'
gem 'handlebars_assets', '~> 0.23.1'
gem 'i18n-js', '~> 3.0'
gem 'sass-rails', '~> 5.0'
gem 'sprockets', '~> 3.7'
gem 'sprockets-rails', '~> 3.2'
gem 'turbolinks', '~> 5.0'
gem 'twbs_sass_rails', '~> 4.5'
gem 'uglifier', '~> 3.2'

group :development, :test do
  gem 'bullet', '~> 5.5'
  gem 'byebug', '~> 9.0'
  gem 'factory_girl_rails', '~> 4.8'
  gem 'faker', '~> 1.7'
  gem 'pry', '~> 0.10.4'
  gem 'pry-byebug', '~> 3.4'
  gem 'pry-rails', '~> 0.3.6'
  gem 'rspec-rails', '~> 3.5'
  gem 'rubocop', '~> 0.48.1', require: false
  gem 'scss_lint', '~> 0.53.0', require: false
  gem 'slim_lint', '~> 0.12.0', require: false
end

group :development do
  gem 'better_errors', '~> 2.1'
  gem 'binding_of_caller', '~> 0.7.2'
  gem 'meta_request', '~> 0.4.0'
  gem 'spring', '~> 2.0'
  gem 'spring-commands-rspec', '~> 1.0'
  gem 'web-console', '~> 3.5'
end

group :test do
  gem 'capybara', '~> 2.13'
  gem 'capybara-screenshot', '~> 1.0'
  gem 'coveralls', '~> 0.8.20', require: false
  gem 'database_cleaner', '~> 1.5'
  gem 'email_spec', '~> 2.1'
  gem 'launchy', '~> 2.4'
  gem 'mongoid-rspec', github: 'mongoid-rspec/mongoid-rspec'
  gem 'poltergeist', '~> 1.14'
  gem 'rspec', '~> 3.5'
  gem 'simplecov', '~> 0.14.1', require: false
  gem 'webmock', '~> 3.0', require: false
end

group :staging, :production do
  gem 'unicorn', '~> 5.3'
end
