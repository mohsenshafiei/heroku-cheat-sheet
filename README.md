### Heroku-Cheat-Sheet

##### Installation
```bash
npm install -g heroku
```

##### Verifying Installation
```bash
heroku --version
```

##### Getting Started and Login
```bash
heroku login
```

##### Creating a Heroku remote
```bash
heroku create
```

##### For an existing Heroku app
```bash
heroku git:remote -a <heroku-app-url>
```

##### Renaming Remotes
```bash
git remote rename heroku heroku-staging
```

##### Deploying Code
```bash
git push heroku master
```

##### Ensure that at least one instance of the app is running
```bash
heroku ps:scale web=1
```

##### Visit the app on the website
```bash
heroku open
```

##### View logs
```bash
heroku log --tail
```

##### Procfile
```bash
web: node index.js
```

##### Check how many dynos are running
```bash
heroku ps
```

##### Scale the number of dynos to n
```bash
heroku ps:scale web=n
```

##### Run the app locally
```bash
heroku local web
```

##### Push local changes
```bash
git push heroku master
```

##### Start a console
```bash
heroku run bash
```

##### Set the config var
```bash
heroku config:set TIMES=2
```
