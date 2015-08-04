source "http://rubygems.org"

# Declare your gem's dependencies in switchman.gemspec.
# Bundler will treat runtime dependencies like base dependencies, and
# development dependencies will be added by default to the :development group.
gemspec

# if put in the gemspec, the :require => false is ignored
gem 'mocha', :require => false

gem 'debugger', platform: :mri_19
gem 'byebug', platform: [:mri_20, :mri_21]

if ENV['RAILS'] == '4.2'
  gem 'activerecord', '~>4.2.3'
  gem 'railties', '~>4.2.3'
elsif ENV['RAILS'] == '4.1' || ENV['RAILS'] == '4'
  gem 'activerecord', '~> 4.1.0'
  gem 'railties', '~> 4.1.0'
elsif ENV['RAILS'] == '4.0'
  gem 'activerecord', '~> 4.0.4'
  gem 'railties', '~> 4.0.4'
else
  gem 'activerecord', '~> 3.2.17'
  gem 'railties', '~> 3.2.17'
end
