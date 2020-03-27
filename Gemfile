# frozen_string_literal: true

source "https://rubygems.org"

ruby RUBY_VERSION

# DECIDIM_VERSION = "0.20"
DECIDIM_VERSION = { git: "https://github.com/decidim/decidim.git", branch: "0.20-stable"}

gem "decidim", DECIDIM_VERSION

gem 'decidim-verifications-csv_email', git: 'https://github.com/CodiTramuntana/decidim-verifications-csv_emails.git'
gem 'decidim-consultations', DECIDIM_VERSION

gem "decidim-decidim_awesome", git: "https://github.com/Platoniq/decidim-module-decidim_awesome"

gem "bootsnap", "~> 1.3"

gem "puma", "~> 3.12.2"
gem "uglifier", "~> 4.1"
gem "faker", "~> 1.9"
gem "figaro"
gem "mail"
gem "sentry-raven"

group :development, :test do
  gem "byebug", "~> 11.0", platform: :mri

  gem "decidim-dev", DECIDIM_VERSION
end

group :development do
  gem "letter_opener_web", "~> 1.3"
  gem "listen", "~> 3.1"
  gem "spring", "~> 2.0"
  gem "spring-watcher-listen", "~> 2.0"
  gem "web-console", "~> 3.5"

  gem 'capistrano'
  gem 'capistrano-rbenv'
  gem 'capistrano-bundler'
  gem 'capistrano-passenger', '>= 0.1.1'
  gem 'capistrano-rails'

end

group :production do
  gem "passenger"
  gem 'delayed_job_active_record'
  gem "daemons"
end
