# steamFFS
Simple use of the steam api to Find Friends' Similar games 

## Running the app
```$ export FLASK_APP=app.py
$ python -m flask run
 * Running on http://127.0.0.1:5000/
```

## References and resources

* [Authentication using steam openID and Flask](http://flask.pocoo.org/snippets/42/)
* [Another one to auth in Flask](https://github.com/positivenoise/Flask-OpenID-Steam)
  They are both the same but they have problems. 
  1. (using python2 so replace urrlib2.urlopen with urllib.request.urlopen and urllib2.encode with urllib.parse.urlencode
  2. SQLAlchemy needs to have the table create at the beggining so need to write `db.create_all()` before running app ( see [here](https://stackoverflow.com/questions/33784212/operationalerror-sqlite3-operationalerror-no-such-table-user))
  3. The authentication doesn't work. Need to try [this](http://python-social-auth-docs.readthedocs.io/en/latest/index.html)
* [Python library to interact with Steam API](https://github.com/smiley/steamapi)
