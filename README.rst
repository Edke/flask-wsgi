Simple flask app with wsgi for testing
======================================

Build
-----

.. code-block:: bash

   $ python setup.py bdist_wheel


Deploy
------

On Debian Buster:

.. code-block:: bash

   $ sudo apt install -y python3 python3-venv virtualenv python3-virtualenv
   $ python3 -m venv /opt/flask-app
   $ /opt/flask-app/bin/python -m pip install /tmp/<oackage>

Run
---

.. code-block:: bash

   $ SEED_USER=johndoe /opt/flask-app/bin/gunicorn flask_app.wsgi
