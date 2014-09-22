# Python 2.7.x Dojo - Code Samples

## Reference code for Flask Hello World

    from flask import Flask
    app = Flask(__name__)
    
    @app.route('/show')
    def hello_world():
        return 'Hello World!'
    
    if __name__ == '__main__':
        app.run()

## Reference code for Decorators

    def reals(func):
        def reals_func(value):
            return 'R$ ' + value
        return reals_func
    
    @reals
    def money_me(string):
        return 'Cost is' + string
    
    print money_me('10')
