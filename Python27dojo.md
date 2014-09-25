# Python 2.7.x Dojo

Build a small system (two software pieces) that will show on a browser the most 5 recent videos from YouTube, and by doing this, learn all through the Python basic concepts.

## Chapter 1 - Basics

### Concepts to understand

- Pip & http://pypi.python.org
  - Pip used to upgrade itself?
  - Pip install libs or software? Or both?
  - What is the difference between a lib and a software?

- Line prompt coding, bpython, ipython, dreampie, and so on...

![Python](images/cmdpython.png) 
![iPython](images/cmdipython.png) 
![bPython](images/cmdbpython.png) 
![DreamPie](images/cmddreampie.png) 

- Indentation is everything. Use 4 spaces
- Maximum line length is 80 characters
- Code in UTF-8 ... ALWAYS!
- Use vi and code like a boss
- How to run a Python 2.7 script
- Virtualenv, Virtualenv, and ... Virtualenv
  - Installing
  - Activating
  - Automation?

![Virtualenv](images/virtualenv.jpg) 

- Data Types
  - Integers
  - Strings
  - Lists
  - Tuples
  - Dictionaries

- Importing modules
- someVar is Java... some_var is Python

## Chapter 2 - Hands on - part I

### To do

- Create and enter into your virtualenv. Call it `env`.
- Use Flask
- "/show" must be the entry point
- Must output any string, like a "hello world"
- Debugging on browser (yep, your code needs to fail)
- Create a new route called "/fail" to return `str(1/0)`

## Chapter 3 - Hands on - part II

### To do

- Create a SEPARATE .py file
- Use Python Requests (you can use the same virtualenv as before)
- FEED: https://gdata.youtube.com/feeds/api/videos?q=a&max-results=5&v=2&alt=jsonc&orderby=published
- Must download and persist the json data on /tmp
- Remember: persist a valid json already serialize. Raw data and raw string will not work.
- Run it on console

## Chapter 4 - Hands on - part III

### To do

- Extend the same software created for chapter 2.
- Use Jinja2 (for templates, its included already by Flask, dont need to install anything)
- You need to use method `render_template` from Flask
- "/videos" must be the entry point
- Must read the json data on /tmp, with exec or by loading its contents (then module json may be helpfull)
- Remember: only pass to template the list of data to be displayed, not the full json object (in this case)
- Must list on the browser the 5 videos, including thumb and a few metadata

## Chapter 5 - Is it clear to read?

### Concepts

- Tabs x Spaces
- PEP8
- Pylint
- How to print your software version?

### To do

- Make your code clear to be read by others

## Chapter 6 - Packaging

### Concepts

- How can I pack my software?
- Egg Package structure
- Code Generators
  - Machete (https://github.com/lovato/machete)
  - CookieCutter (https://github.com/audreyr/cookiecutter)

### To do

- Code everything again, using Machete templates

## Chapter 7 - Testing

- Nose

## Chapter 8 - Final Concepts

- Egg x Wheel
- pip install (Install from everywhere)
- virtualenvwrapper
- cron: to use or not?
- filtros jinja
- decorators
- Upload my software to Pypi
- Boilerplates & Bootstrap (shortcuts)
- flask-bootstrap
- Python is not Java ... forget getters and setters (http://typicalprogrammer.com/doing-it-wrong-getters-and-setters/)

## Chapter 9 - To space and beyond

- GAE
- http://www.rafekettler.com/magicmethods.pdf
