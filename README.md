# React with Ruby on Rails

### Setup
* [Install Ruby and Rails](https://gorails.com/setup/osx/10.15-catalina)
* [Install Postgres](https://postgresapp.com)
* [Install the Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli)

### App initialization
```
rails new appname --webpack=react -d=postgresql
rails g controller pages index
```

### React components
```
yarn add react-piano
yarn add soundfont-player
yarn add react-dimensions
```

### Database initialization
```
rake db:create
rake db:migrate
```

### Deployment (using Heroku CLI)
```
git add .
git commit -m "commit message"
heroku create
git push heroku master
heroku open
```


### Next steps, for a simple app to save and play back melody ideas:
* Add react-router
* Adding navigation and basic styles (Bootstrap or many other good options)
* Create a User model and a Song model, with a song containing a sequence of notes as returned by the react-piano component. Choose a gem for easy setup of user account authentication with encrypted keys
* user has_many songs (ActiveRecord association)
* API endpoints for POST and GET user/songs
* Refactor into a Keyboard component with recording and playback functionality (already included in react-piano), hook up to the API endpoints and we're good to go
* After another hour or two of work, we could have a full app up and running that allows people to record and play back piano ideas. Pretty neat!

Thanks to Kevin Qi for the react-piano component and to Zayne for his excellent tutorials introducing this app architecture.
