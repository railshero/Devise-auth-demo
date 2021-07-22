# Authentication with devise:demo/tutorial

## Gems
* devise
* letter_opener

## Versions
* Ruby: 3.0.1
* Rails:  6.1.4


## Running
1. Run bundler
```
bundle install
```
2. Run migrations
```
rails db:migrate
```
3. Start rails server
```
rails s
```

Please change 
```config.mailer_sender = 'no-reply@example.com```
in config/initializers/devise.rb

Check Out [Devise Beginners Tutorial](https://railshero.pw/406/for-beginners-authentication-with-devise)

[RailsHero](https://railshero.pw)