This is an out-of-the box runnable Facebook app built on Rails 3. Just plugin your Facebook ID and keys and you're good to go.

It uses Devise, OmniAuth and the omniauth-facebook strategy.

To customize, replace MyAwesomeFacebookApp with your app name on these files:
Rakefile
config.ru
app/views/layouts/application.html.erb
config/application.rb
config/environment.rb
config/environments/development.rb
config/environments/production.rb
config/environments/test.rb
config/initializers/secret_token.rb
config/initializers/session_store
config/routes.rb

Edit config/initializers/devise.rb. Change this line:
  config.omniauth :facebook, "APP_ID", "APP_SECRET"

and put in your actual Facebook app ID and app secret.

References:
https://github.com/plataformatec/devise/wiki/OmniAuth:-Overview
https://github.com/intridea/omniauth/wiki/List-of-Strategies
https://github.com/mkdynamic/omniauth-facebook
https://github.com/mkdynamic/omniauth-facebook/blob/master/example/config.ru
http://railsapps.github.com/tutorial-rails-devise-rspec-cucumber.html
