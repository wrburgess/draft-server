source "https://rubygems.org"

ruby "2.0.0"
gem "rails", "4.0.0"

gem "coveralls", "0.6.7", require: false
gem "devise", "3.0.3"
gem "faker", "1.2.0"
gem "json", "1.8.0"
gem "nokogiri", "1.6.0"
gem "pg", "0.16.0"
gem "resque", "1.24.1", require: "resque/server"
gem "settingslogic", "2.0.9"
gem "uglifier", "2.2.1"
gem "unicorn", "4.6.3"

group :production do
  gem "rails_12factor", "0.0.2"
end

group :development do
  gem "better_errors", "0.9.0"
  gem "binding_of_caller", "0.7.2"
  gem "tracer_bullets", "0.0.5"
end

group :development, :test do
  gem "capybara", "2.1.0"
  gem "database_cleaner", "1.1.1"
  gem "debugger", "1.6.1"
  gem "dotenv-rails", "0.9.0"
  gem "factory_girl_rails", "4.2.1"
  gem "fuubar", "1.2.1"
  gem "pry-rails", "0.3.2"
  gem "pry-remote", "0.1.7"
  gem "rspec-rails", "2.14.0"
  gem "shoulda", "3.5.0"
end