
Running the app locally
=======================

Sometimes you need to present your talk without an internet connection.
In this situation you can run a local web server::

  $ virtualenv venv
  $ source venv/bin/activate
  (venv)$ pip install git+https://github.com/bast/cicero.git@master#egg=cicero
  (venv)$ cicero

  * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)


How to preview and serve your talk locally
==========================================

Using a local server it is also no problem to serve your talk locally to see the
result before you push them to the repository::

  $ cicero --file /home/user/my-talk/talk.md


Development
===========

First install the dependencies (you need a network connection for this step)::

  $ git checkout https://github.com/bast/cicero
  $ cd cicero
  $ pipenv install

Then start the server::

  $ pipenv run python cicero.py

  * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
