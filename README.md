# sample_app

This is a Rails 5 app.

## Usage

```terminal
$ git clone https://github.com/rocLv/SampleApp.git
$ cd SampleApp
$ bundle install
$ rails db:create db:migrate

```


## Prerequisites

This project requires:

* Ruby 2.4.1, preferably managed using [rbenv][]
* Chromedriver for Capybara testing
* PostgreSQL must be installed and accepting connections
* [Redis][] must be installed and running on localhost with the default port

On a Mac, you can obtain all of the above packages using [Homebrew][].

If you need help setting up a Ruby development environment, check out this [Rails OS X Setup Guide](https://mattbrictson.com/rails-osx-setup-guide).

## Getting started

### bin/setup

Run the `bin/setup` script. This script will:

* Check you have the required Ruby version
* Install gems using Bundler
* Create local copies of `.env` and `database.yml`
* Create, migrate, and seed the database

### Run it!

1. Run `bin/rake test` to make sure everything works.
2. Run `bin/rake test:system` to run system (capybara) tests.
3. Run `bin/rails s` to start the Rails app.
4. In a separate console, run `bin/sidekiq` to start the Sidekiq background job processor.

[rbenv]:https://github.com/sstephenson/rbenv
[redis]:http://redis.io
[Homebrew]:http://brew.sh
