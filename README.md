Welcome to PRODROMUS, a very tiny XMPP client.
==============================================

"Hey there, I'm *PRODROMUS*, a *very simple XMPP messaging client*, mainly reasonable as contact
form replacement/supplement or support contact utility."

"Prodromus" is Latin and means as much as "express messenger", "courier". Prodromus makes use of
the great [Strophe.js](http://strophe.im/strophejs/) library. It also uses [jQuery](http://jquery.com/).

Visit the [projekt wiki](http://forge.webpresso.net/projects/prodromus/wiki/Wiki) for more information
as well as a screencast.

Requirements
------------

The client itself only requires JavaScript and a BOSH endpoint. The endpoint has to be reachable
on the same domain as PRODROMUS was accessed due to JavaScript cross-domain restrictions. The
simplest way is to set up a reverse proxy with Apache's mod_proxy - see the
[contents/example.htaccess](http://forge.webpresso.net/projects/prodromus/repository/revisions/master/entry/contents/htaccess.sample)
example file.

Another requirement is a XMPP server with SASL anonymous enabled.


Installation
------------

# [Download PRODROMUS](http://forge.webpresso.net/projects/prodromus/files).
# Copy the files to your web server.
# Ensure a BOSH endpoint / [connection manager](http://metajack.im/2008/09/08/which-bosh-server-do-you-need/)
  is accessible under the same domain you access PRODROMUS. If you're using Apache you can enable mod_proxy,
  rename the source:contents/htaccess.sample to .htaccess and adjust the URL of your BOSH-Service. ejabberd,
  for example, already comes with built-in BOSH support.
# Open contents/prodromus.js and configure PRODROMUS to fit your needs. The following values are important:
  XMPP_SERVER, BOSH_SERVICE and RECEIVER. You can also configure the date format and language, currently English
  ("en") and German ("de") are supported.
# You should be ready to go. Try it by opening prodromus.html in your browser. You can integrate PRODROMUS into
  your website later.


Bug tracker
-----------

Bugs are tracked in the project Redmine installation:
https://forge.webpresso.net/projects/prodromus/issues


Source code
-----------

The source code of the application can be found in a Git repository. Browse it
online (https://forge.webpresso.net/projects/prodromus/repository) or

`git clone https://code.webpresso.net/git/prodromus`


Authors
-------

**Raphael Kallensee**

+ http://raphael.kallensee.name
+ http://identi.ca/rkallensee
+ http://twitter.com/rkallensee


License
---------------------

Copyright 2011-2012 Raphael Kallensee.

[![AGPLv3](http://www.gnu.org/graphics/agplv3-155x51.png)](http://www.gnu.org/licenses/agpl-3.0.html)

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU Affero General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
