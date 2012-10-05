This is a very simple (and ugly) implementation of the well known mine
sweeper type game, in the Pylons framework. No extra dependencies are 
needed above Pylons itself, except for easy_install.

Installation and Setup
======================

Install ``Sweepy`` using easy_install::

    easy_install Sweepy

Make a config file as follows::

    paster make-config Sweepy config.ini

Tweak the config file as appropriate and then setup the application::

    paster setup-app config.ini

Then you are ready to go.

Running Sweepy
==============

Assuming you have permissions to run a webserver on port 80 of your local 
machine:

    paster serve config.ini

The game is now available at http://localhost .

If not, you need to edit config.ini and change the port under the [server:main]
section to a port you have permissions to use. This will usually be a port 
above 1024, e.g. 8000; and in that case the game is available at 
http://localhost:8000
