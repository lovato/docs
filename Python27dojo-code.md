# Python 2.7.x Dojo - Code Samples

## Reference code for Flask Hello World

    # -*- coding: utf-8 -*-
    from flask import Flask
    app = Flask(__name__)
    
    @app.route('/show')
    def hello_world():
        return 'Hello World!'
    
    if __name__ == '__main__':
        app.run()

## Reference code for Requests

    # -*- coding: utf-8 -*-
    import requests
    url = 'https://gdata.youtube.com/feeds/api/videos?q=a&max-results=5&v=2&alt=jsonc&orderby=published'
    r = requests.get(url)
    if r.status_code == 200:
        print r.text

## Reference code for Decorators

    def reals(func):
        def reals_func(value):
            return 'R$ ' + value
        return reals_func
    
    @reals
    def money_me(string):
        return 'Cost is ' + string
    
    print money_me('10')
