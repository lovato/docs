# Python 2.7.x Dojo - Code Samples

## Referemce code for Flask Hello World

from flask import Flask
app = Flask(__name__)

@app.route('/show')
def hello_world():
    return 'Hello World!'

if __name__ == '__main__':
    app.run()
