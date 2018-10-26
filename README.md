This project is about setting up a ubuntu instance and deploy a web application using apche web server.
The linux machine is hosted by AWS lightsail.

Modifications @ ubuntu instance:
- create user grader
- give grader sudo rights
- create 2 key pairs, one for ubuntu one for grader
- disable ssh password auth
- change ssh port from 22 to 2200
- update the system using apt-get update/upgrade
- set up ufw (default deny in, default allow out, enabled ports: ssh(2200), HTTP(80), NTP(123))

