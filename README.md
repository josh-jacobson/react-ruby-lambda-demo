# React with Ruby on Rails

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

### Setup
* [Install Ruby and Rails](https://gorails.com/setup/osx/10.15-catalina)
* [Install Postgres](https://postgresapp.com)
* [Install the Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli)

### App initialization
```
rails new appname --webpack=react -d=postgresql
rails g controller pages index
```

* Database initialization
```
rake db:create
rake db:migrate
```

* Deployment (using Heroku CLI)
```
git add .
git commit -m "commit message"
heroku create
git push heroku master
heroku open
```

Thanks to Kevin Qi for the react-piano component and to Zayne for his excellent tutorials introducing this app architecture.
