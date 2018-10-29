This project is about setting up a ubuntu instance and deploy a web application using apche web server.
The linux machine is hosted by AWS lightsail.

The server can be reached at 52.59.29.113 at port 2200.


Modifications @ ubuntu instance:
- create user grader
- give grader sudo rights
- create 2 key pairs, one for ubuntu one for grader
- disable ssh password auth
- change ssh port from 22 to 2200
- update the system using apt-get update/upgrade
- set up ufw (default deny in, default allow out, enabled ports: ssh(2200), HTTP(80), NTP(123))
- git already installed
- changed owner and group of var/www/itemCatalog to www-data to be able to write to the db


Software & packages:
with apt:
- installed apache (apache2)
- installed pyhton3 wsgi module for apache (libapache2-mod-wsgi-py3)
- installed python2 wsgi module for apache (libapache2-mod-wsgi)
- installed sqlite (sqlite)
- installed sqlalchemy (python-sqlalchemy)
- installed passlib (python-passlib)
- installed pip (python-pip)
- installed pip3 (python-pip3)
- installed flask http authentification (python-flask-httpauth)

with pip:
- installed google module for google OAuth (google-cloud-storage)
- installed flask (flask)
- installed httplib2 (httplib2)
- installed flask http authentification (Flask-HTTPAuth)


