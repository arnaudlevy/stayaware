# README

```
git clone git@github.com:arnaudlevy/stayaware.git
rails new stayaware -d postgresql
cd stayaware/
rails s
rails db:create # Si erreur
git status
git add .
git commit -am "init"
git push
rails g scaffold Site name:string url:string
rails db:migrate
git status
git add .
git commit -am "sites"
git push
```

Création de l'app sur Heroku, puis:
```
heroku git:remote -a stayaware
git push heroku master
heroku run rails db:migrate
```