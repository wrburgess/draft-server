# draft-server

[![Build Status](https://travis-ci.org/wrburgess/draft-server.png)](https://travis-ci.org/wrburgess/draft-server)
[![Dependency Status](https://gemnasium.com/wrburgess/draft-server.png)](https://gemnasium.com/wrburgess/draft-server)
[![Code Climate](https://codeclimate.com/github/wrburgess/draft-server.png)](https://codeclimate.com/github/wrburgess/draft-server)
[![Coverage Status](https://coveralls.io/repos/wrburgess/draft-server/badge.png)](https://coveralls.io/r/wrburgess/draft-server)

## style

* use double quotes ```"``` whenenver possible

## security

### secret key replacement

* use ```rake secret``` to generate a new secret key for your app  
* add ```APP_SECRET_KEY_BASE=XXXXXXXXX``` to your ```.env``` file  
* add the new environment variable to replace the original secret key

```
# config/initializers/secret_token.rb

DraftServer::Application.config.secret_key_base = ENV["APP_SECRET_KEY_BASE"]```
```

* add the new secret key to your heroku staging and production environments

```heroku config:set APP_SECRET_KEY_BASE=XXXXXXXXX --remote staging```
```heroku config:set APP_SECRET_KEY_BASE=XXXXXXXXX --remote production```

## models

* draft
* pick
* roster
* slot
* piece
* user

## foreman setup

## travis setup

## settingslogic setup

## dot-env setup

## heroku setup

### staging and production environments

* establish designations for your staging app

```heroku config:set RACK_ENV=staging RAILS_ENV=staging --remote staging```

* set up a staging.rb file in your environments directory

```git cp config/environments/production.rb config/environments/staging.rb```