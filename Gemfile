if RUBY_VERSION =~ /1.9/
   Encoding.default_external = Encoding::UTF_8
   Encoding.default_internal = Encoding::UTF_8
end

source 'http://rubygems.org'

gem 'mysql2',   '0.3.11'     if ENV['DB'].nil? || ENV['DB'] == "mysql"
gem 'sqlite3',  '1.3.5'     if ENV['DB'].nil? || ENV['DB'] == "sqlite"
gem 'pg',       '0.11.0'    if ENV['DB'].nil? || ENV['DB'] == "postgres"

gem 'rails',                '3.2.1'
gem 'jquery-rails',         '1.0.18'
gem 'string-utils',         '0.2.0'
gem 'omniauth',             '1.0.0'
gem 'devise',               '1.5.0'
gem 'ancestry',             '1.2.4'
#gem 'acts_as_list',         '0.1.4'
gem 'cancan',               '1.6.7'
gem 'gravatar_image_tag',   '1.0.0'
gem 'themes_for_rails',     '0.4.3'
gem 'cells',                '3.8.0'
gem 'cells-filters',        '0.0.1'
gem 'paperclip',            '2.4.5'
#gem 'ckeditor',             '3.7.0.rc2'
gem 'ckeditor',             :path => 'vendor/gems/ckeditor'
gem 'acts_as_commentable',  '3.0.1'
gem 'recaptcha-rails3',     '0.3.4', :require => "recaptcha/rails"
gem 'will_paginate',        '3.0.2'
gem "comma",                '~> 3.0' # CSV export
gem 'fastercsv',            :platforms => :ruby_18

# For deploying on Heroku
# gem 'heroku', '2.14.0'
# gem 'aws-s3', '0.6.2'

# Example of snippet got via external gem ## broken in production due to bluecloth
# gem 'railsyard-markdown-content', :path => 'vendor/gems/railsyard-markdown-content'

group :development, :test do
  gem 'rspec',              '2.8.0'
  gem 'rspec-rails',        '2.8.1'
  gem 'cucumber',           '1.1.4'
  gem 'cucumber-rails',     '1.2.1'
  gem 'webrat',             '0.7.3'
  gem 'capybara',           '1.1.2'
  gem 'ruby-debug',         '~> 0.10.4' if RUBY_VERSION =~ /1.8/
  gem 'ruby-debug19',       '~> 0.11.6' if RUBY_VERSION =~ /1.9/
  #gem 'capybara-firebug',   '0.0.10'
  gem 'deadweight',         '>=0.2.1'
  gem 'launchy'
  gem 'database_cleaner',   '0.7.1'
  gem 'factory_girl'
  gem 'railroady'
  # you don't need guard to test on travis
  unless ENV['TRAVIS']
    gem 'guard'
    gem 'guard-cucumber'
  end
end
