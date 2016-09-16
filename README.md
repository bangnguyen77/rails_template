# RAILS TEMPLATE

This is a template for Ruby on Rails with gems: bootstrap-sass, devise and some testing tools are installed.

* Ruby version: Ruby 2.2.2 or higher and Rails 5.0.0

* Create a new project
```
rails new rails_template -d postgresql -T
```
* -d postgresql tells Rails to use Postgres for the database,
and -T tells it not to install its testing tools - by default, it uses a library called test-unit, whereas we use RSpec

* finalize testing setup for Rspec and Shoulda Matchers
```
rails generate rspec:install
```
* Then we can create our databases with:
```
rails db:create
```
* Then we create our Posts table (just as example) with:
```
rails g migration create_lists for short
```
* Then we can migrate, and prepare our test database, and Active Record will create the schema.rb file in db.
```
  rails db:migrate
  rails db:test:prepare
```
* In a new terminal, start the postgres server:
```
$ postgres
```

* Finally, to start the Rails server, we run $ rails server in our project folder. This is where our server logs will be written. We can take a look at the default page served by navigating to localhost:3000.
