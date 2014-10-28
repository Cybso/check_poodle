check\_poodle
============

Nagios/Icinga Plugin that checks for SSLv2 and SSLv3 support

Uses OpenSSL s\_client to perform support checks for SSLv2 and SSLv3
or STARTTLS/SSLv2, SSLv3 on various services.

Installation
------------

* Copy bin/check\_poodle into /usr/local/bin/check\_poodle and make it 
  executable.
* Copy services/poodle into /etc/nagios/objects/services (or
  /etc/icinga/objects/services) and modify the files for your need. 
  They expect a hostgroup named 'all'.
* Restart Nagios/Icinga.

Checked services
----------------

At the moment, the following ports are queried:

* Port 443 (HTTPS)
* Port 465 (SMTPS)
* Port 636 (LDAPS)
* Port 993 (IMAPS)
* Port 995 (POP3S)
* Port 5223 (XMPP)
* Port 25 (SMTP, STARTTLS)
* Port 587 (SMTP, STARTTLS)
* Port 143 (IMAP, STARTTLS)
* Port 110 (POP3, STARTTLS)
* Port 5222 (XMPP, STARTTLS)
* Port 5269 (XMPP, STARTTLS)
* Port 20 (FTP, STARTTLS)
* Port 21 (FTP, STARTTLS)

