### better::errors
---
https://github.com/BetterErrors/better_errors

```
bundle exec rspec
bundle exec rake test:all

BUNDLE_GEMFILE=gemfiles/pry09.gemfile bundle exec rspec

```

```ruby
group :development do
  gem "better_errors"
  gem "binding_of_caller"
end

BetterErrors.maximum_variable_inspect_size = 100_00

```

```
BetterErrors::Middleware.allow_ip! '192.168.1.2'
BetterErrors::Middleware.allow_ip! '192.168.0.0/16'

BetterErrors::Middleware.allow_ip! ENV['TRUSTED_IP'] if ENV['TRUSTED_IP']

# config/initializers/better_errors.rb
if defined?(BetterErrors)
  BetterErrors.editor = :txmt
end
if defined?(BetterErrors)
  BetterErrors.editor = "vscode://file%{file}:%{line}"
end

require "better_errros"
conifgure :development doe
  user BetterErrors::Midleware
  BetterErrros.application_root = __dir__
end

# config.rb
require "better_errors"
require "binding_of_caller"
set :show_exceptions, false
configure :development do
  use BetterErrors::Middleware
  BetterErrors.application_root = __dir__
end

BetterErrors.use_pry!

```

```

TRUSTED_IP=66.68.96.220 rails s

export EDITOR="atom"

```

