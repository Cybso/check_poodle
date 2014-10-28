check\_poodle
============

Nagios/Icinga Plugin that checks for SSLv3 support

Uses OpenSSL s\_client to perform support checks for SSLv3
or STARTTLS/SSLv3 on various services.

Installation
------------

* Copy bin/check\_poodle into /usr/local/bin/check\_poodle and make it 
  executable.
* Copy services/poodle into /etc/nagios/objects/services (or
  /etc/icinga/objects/services) and modify the files for your need. 
  They expect a hostgroup named 'all'.
* Restart Nagios/Icinga.
