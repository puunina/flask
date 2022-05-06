# flask
Basic knowladge about flask and some bootstrap. Simple project.

tutorial created by Jim from JimShapedCoding https://www.youtube.com/watch?v=Qr4QMBUPxWo

flask documentation https://flask.palletsprojects.com/en/2.1.x/

1.  py -3 -m venv <name_environment> >> new virtual environment
    python3 -m venv <name_environment>

2.  <name_environment>/bin/activate >> linux
    <name_environment>\Scripts\activate >> Windows

3. pip3 install flask
    pip3 freeze >> installed

4. quickstart https://flask.palletsprojects.com/en/2.1.x/quickstart/

from flask import Flask

app = Flask(__name__)

@app.route("/")
def hello_world():
    return "<p>Hello, World!</p>"

5.  export FLASK_APP = name_of_our_file.py >> linux
    setx FLASK_APP "name_of_our_file.py" >> windows
