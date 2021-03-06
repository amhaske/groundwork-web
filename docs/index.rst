.. highlight:: python
   :linenothreshold: 5

.. image:: https://img.shields.io/pypi/l/groundwork-web.svg
   :target: https://pypi.python.org/pypi/groundwork-web
   :alt: License
.. image:: https://img.shields.io/pypi/pyversions/groundwork-web.svg
   :target: https://pypi.python.org/pypi/groundwork-web
   :alt: Supported versions
.. image:: https://readthedocs.org/projects/groundwork-web/badge/?version=latest
   :target: https://readthedocs.org/projects/groundwork-web/
.. image:: https://travis-ci.org/useblocks/groundwork-web.svg?branch=master
   :target: https://travis-ci.org/useblocks/groundwork-web
   :alt: Travis-CI Build Status
.. image:: https://coveralls.io/repos/github/useblocks/groundwork-web/badge.svg?branch=master
   :target: https://coveralls.io/github/useblocks/groundwork-web?branch=master
.. image:: https://img.shields.io/scrutinizer/g/useblocks/groundwork-web.svg
   :target: https://scrutinizer-ci.com/g/useblocks/groundwork-web/
   :alt: Code quality
.. image:: https://img.shields.io/pypi/v/groundwork-web.svg
   :target: https://pypi.python.org/pypi/groundwork-web
   :alt: PyPI Package latest release

.. _groundwork: https://groundwork.readthedocs.io

Welcome to groundwork web
=========================

groundwork-web provides web app management functions to applications based on the framework `groundwork`_.

.. sidebar:: groundwork framework

   `groundwork`_ is a plugin based Python application framework, which can be used to create various types of applications:
   console scripts, desktop apps, dynamic websites and more.

   Visit `groundwork.useblocks.com <http://groundwork.useblocks.com>`_
   or read the `technical documentation <https://groundwork.readthedocs.io>`_ for more information.

It provides the management of the following objects:

* **Routes**: Define URLs and map functions for rendering froms, templates and more.
* **Contexts**: Group routes and use common folders and configurations.
* **Menus**: Define menus and sub-menus for webpages
* **Servers**: Register own server configurations for easy and fast starts.
* **Database Table Views**: Register database tables to get generated views for editing database content via web forms.
* **Database Table REST Views** Get access to database table content via a REST API.

Besides this, the integrated plugins provides functions for:

* starting a ready-to-use **flask-debug server**
* using a **bootstrap-based template** with integrated menus
* getting web views of detailed information about registered **groundwork objects** like plugins, commands,
  signals, routes and more.

This package contains the following applications, plugins or patterns:

Applications
------------
GroundworkWebApp
~~~~~~~~~~~~~~~~
Example application, which mainly loads the plugin :ref:`gwweb` and :ref:`gwwebmanager`

Plugins
-------
GwWeb
~~~~~
Provides command line commands to show and start web servers. Configures also the web server "flask_debug".

GwWebManager
~~~~~~~~~~~~
Provides web views and functions to manage groundwork objects like commands, recipes, signals, web routes and more.
Allows the user to get a fast overview about the running applications and its configuration.

Patterns
--------
GwWebPattern
~~~~~~~~~~~~
Allows plugins to register web routes and servers.
Cares about the correct setup of `flask <http://flask.pocoo.org/>`_, on which most groundwork web functions are based on.

GwWebDbAdminPattern
~~~~~~~~~~~~~~~~~~~
Allows the registration of database tables to provide admin web views for them.
This enables you to create, read, update and delete (CRUD) content of database tables via a web interface.

GwWebDbRestPattern
~~~~~~~~~~~~~~~~~~
Allows the registration of database tables to provide a REST interface for them.
This enables you to create, read, update and delete (CRUD) content of database tables via a REST interface.

Table of content
----------------

.. toctree::
   :maxdepth: 2

   installation
   architecture
   applications
   plugins
   patterns