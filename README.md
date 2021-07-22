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

## Using in Development
Devise's outgoing mails will be displayed using letter_opener. letter_opener will open generated mails in a new browser window.

## Using In Production
Add Environment Variables for
SMTP_SERVER, SMTP_PORT, SMTP_USERNAME and SMTP_PASSWORD
```
config.action_mailer.smtp_settings = {
    :address              => ENV['SMTP_SERVER'],
    :port                 => ENV['SMTP_PORT'],
    :user_name            => ENV['SMTP_USERNAME'],
    :password             => ENV['SMTP_PASSWORD'],
    :authentication       => :login,
    :tls                  => :true,
    :enable_starttls_auto => true
  }
```  


Check Out [Devise Beginners Tutorial](https://railshero.pw/406/for-beginners-authentication-with-devise)

[RailsHero](https://railshero.pw)