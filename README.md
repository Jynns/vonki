## Enter venv
source venv/bin/activate

### extension in venv
flask-wtf\
flask-sqlalchemy\
flask-migrate\
email-validator

## Run flask
enter venv\
command: export FLASK_APP=vonki.py\
command: flask run

## Deployment
set FLASK_DEBUG=0 in .flaskenv\
add secret key\
add SQLALCHEMY_DATABASE_URI entry\
configure mail service in config.py

## development
export FLASK_DEBUG=1\
export MAIL_SERVER=localhost\
export MAIL_PORT=8025\
command to run smtp server locally: aiosmtpd -n -c aiosmtpd.handlers.Debugging -l localhost:8025


## Database
### migrate changes
flask db migrate -m ""\
flask db upgrade
### reset content
sh clear_db.sh