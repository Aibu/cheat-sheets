## Heroku

### Run terminal in Heroku dyno
```
heroku run bash
```
### Print Heroku env constants
```
heroku config
```
### Set Heroku env constant
```
heroku config:set <env-name>=<env-value>
```

## Run Postico with a remote Heroku PostgreSQL database:
Install this Heroku plugin: [heroku-postico](https://www.npmjs.com/package/heroku-postico) 
```
heroku plugins:install heroku-postico
```
Open Postico with connection to the current app PostgreSQL db:
```
heroku postico:open
```


[Go back to the Cheat Sheets menu.](../README.md)
