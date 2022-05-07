# flask
Basic knowladge about flask and some bootstrap. Simple project.

tutorial created by Jim from JimShapedCoding https://www.youtube.com/watch?v=Qr4QMBUPxWo

flask documentation https://flask.palletsprojects.com/en/2.1.x/

1.  py -3 -m venv <name_environment> >> new virtual environment
    python3 -m venv <name_environment>

2.  <name_environment>/bin/activate >> linux
    <name_environment>\Scripts\activate >> Windows

3.  pip3 install flask
    pip3 freeze >> requirements.txt installed libraries

4. quickstart https://flask.palletsprojects.com/en/2.1.x/quickstart/

from flask import Flask

app = Flask(__name__)

@app.route("/")
def hello_world():
    return "<p>Hello, World!</p>"

5.  export FLASK_APP = name_of_our_file.py >> linux
    setx FLASK_APP "name_of_our_file.py" >> windows + restart!!

6. flask run
7. setx FLASK_DEBUG "1"

Libraries:
1. sqlalchemy >> bazy
from flask_sqlalchemy import SQLAlchemy
db = SQLAlchemy(app)
2. flask_bcrypt >> for passwords https://flask-bcrypt.readthedocs.io/en/1.0.1/
3. flask_login
4. flask_wtf > forms >forms.py
from flask_wtf import FlaskForm
5. email_validator

baza
In virtualenv:
1. python
2. from file import db
3. db.create_all() >> creates database ussing our class Item(db.Model)
4. from file import Item >> adds element to our database
object = Item(name="laptop, price = 500,..................)
db.session.add(object)
db.session.commit()
5. item.query.all() >> displays all element in database