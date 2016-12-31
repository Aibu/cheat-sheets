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

### Run Postico with a remote Heroku PostgreSQL database:
Install this Heroku plugin: [heroku-postico](https://www.npmjs.com/package/heroku-postico) 
```
heroku plugins:install heroku-postico
```
Open Postico with connection to the current app PostgreSQL db:
```
heroku postico:open
```

### Clean up node_modules cache
```
heroku config:set NODE_MODULES_CACHE=true
git commit -am 'rebuild' --allow-empty
git push heroku master
heroku config:unset NODE_MODULES_CACHE
```

### Log node without PostgreSQL
```
heroku logs --tail | grep -v 'Executing'
```
where the -v parameter inverts the grep search, so that only other log messages are shown (assuming they don't have the text 'Executing' in their content).


[Go back to the Cheat Sheets menu.](../README.md)
