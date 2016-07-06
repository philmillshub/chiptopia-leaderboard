# chiptopia-leaderboard

This is a basic leaderboard app made with sinatra. It's used to show your friends' Chipotle Chiptopia status. It's pretty simple to host on Heroku.

Run locally:
```
export CARDS='base64-encoded-yaml-from-example-with-your-chiptopia-cards'
bundle install
bundle exec ruby app.rb
```

Needed to deploy to heroku
```
heroku config:set CARDS='???'
```

Example YAML format:
```yaml
nickname:
  'card-number'
othernickname:
  'another-chiptopia-card-number'
```

Take the YAML and Base64 encode it as the CARDS env var.
