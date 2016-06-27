# cherrypy-heroku-example

A very minimal example that can be used for doing quick web prototyping in Python. 

## About

This is especially designed for people who have an understanding of Python but are new to web development in particular. It can be difficult to decide on components and frameworks so that you can get down to coding. This example uses [cherrypy](http://www.cherrypy.org/) for the webserver, [jinja2](http://jinja.pocoo.org/docs/dev/) for html rendering, and provides a Procfile so that it can be immediately deployed on [Heroku](https://heroku.com).

## Setting up locally

Make sure you have [Python](https://www.python.org/) and [pip](https://pip.pypa.io/en/stable/installing/) installed.

```bash
git clone https://github.com/mispy/cherrypy-heroku-example.git
cd cherrypy-heroku-example
pip install -r requirements.txt
python app.py
```

The webserver should now be running on http://localhost:5000. Editing app.py will cause cherrypy to reload itself.

## Deploying to Heroku

Install the [Heroku toolbelt](https://toolbelt.heroku.com/), and make sure you commit your changes to git. Now you can deploy:

```bash
heroku create
git push heroku master
```

If all goes well, you can open your app in the browser:

```bash
heroku open
```
