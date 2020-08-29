source 'https://rubygems.org'

gemspec

gem 'money', git: 'https://github.com/levelone/money', tag: 'v6.13.8.rc1'

platforms :jruby do
  gem "activerecord-jdbc-adapter"
  gem "activerecord-jdbcsqlite3-adapter"
  gem "jruby-openssl"
end

platforms :ruby do
  gem "sqlite3"
end

platform :mri do
  # gem "ruby-prof", "~> 0.11.2"

  case RUBY_VERSION
  when /^1.9/
    gem 'debugger'
  end
end

group :development do
  gem "pry"
  gem 'rb-inotify', '~> 0.9'
  gem 'guard'
  gem 'guard-rspec'
  gem 'guard-rails'
end
