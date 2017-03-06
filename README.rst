=============================
Transfer from Trac to Redmine
=============================

These Jupyter Notebook files helps to transfer data between a Trac Instance and a Redmine Project.

Install
=======

To setup please create a Python virtualenv and install the requirements.

.. code:: bash

    python3 -m venv .
    ./bin/pip install -U -r requirements.txt

Setup
=====

To setup the notebooks, start them

.. code:: bash

    ./bin/jupyter-notebook

In the Notebooks adjust the trac and redmine settings

.. code:: python
    # Setup Redmine-Connector:
    redmine = Redmine(
        'https://demo.redmine.org/',
        key='<actuale key from Redmine API>'
    )
    redmine_project = '<project name>'

    # Trac Settings
    trac_url = "https://demo.trac.org/"
    trac_project = "project"

    trac_user = "<user name>"
    trac_password = "<password>"

execute all cells.
