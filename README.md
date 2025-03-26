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
add secret key\
add SQLALCHEMY_DATABASE_URI entry

## Database
### migrate changes
flask db migrate -m ""\
flask db upgrade
### reset content
sh clear_db.sh