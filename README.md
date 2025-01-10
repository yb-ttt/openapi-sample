# README

This is a repository example of the issue: https://github.com/mkon/openapi_contracts/issues/98

Steps:

1. Start a new project with 

```sh
$ rails new openapi-sample --api

```

2. Go through RSpec installation

```ruby
# Gemfile
group :development, :test do
 ...
  gem "rspec-rails"
  
end
```

```sh
$ bundle install
```

```sh
$ rails generate rspec:install
```

3. Add `openapi_contracts` gem in the project

```ruby
# Gemfile
group :development, :test do
 ...
  gem "rspec-rails"
  gem "openapi_contracts"  
end

```

Run bundle install again

```sh
$ bundle install
```

4. Run the desired command
```sh
$ bin/rails db:test:prepare test
```