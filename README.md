# Fora

Fora is a multi-user video chat app, built using Rails, Stimulus and the Vonage SDK.  It is spefically designed with remote learning in mind.

At the moment, there is not much going on in terms of features though!

## Getting started

* You'll need to sign up for a free account at [vonage].  Once you've done that, get the api key and secret and stick them in your .bash_profile, or an equivalent location, so that the application can pick up ENV['VONAGE_API_KEY'] and ENV['VONAGE_API_SECRET'].

* Install the dependencies with `bundle install`

* If you run into problems with webpacker, try

```
bundle exec rails webpacker:install
rails webpacker:compile
```

* Also make sure the db is created and migrated

```
rails db:create db:migrate
```

* Then you'll need to create at least one user.  You can either do that in the rails console or through the application GUI.

* To fire up the application do `rails s`

* By default, the application will run on `localhost:3000`

[vonage]: https://www.vonage.co.uk/communications-apis/video/