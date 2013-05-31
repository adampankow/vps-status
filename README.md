vps-status
============

A Server (VPS) Monitor that I made to quickly check the status of my [FlipHost VPS](http://www.fliphost.net/vps.html). Uses [SolusVM Client API](http://docs.solusvm.com/client_api). Your VPS provider must provide this, if it's not something they have, this is probably of zero interest to you.


What It Does
============

Shows you weather or not your chosen server is online, disk usage, RAM usage, and bandwidth usage. You can see [a demo on Heroku](http://status.longren.org/). Click the button to refresh the page. You can also press the 'r' key on your keyboard to refresh. 

There's also an option in config.php to enable live updating of values via ajax. To enable, set ```PHP $dynamicUpdates = true;``` in config.php and refresh your page.


What It Doesn't Do
==================

It won't notify you about anything.


How To Use It
=============

Upload the files to your webserver. Change values in config.php to match your client api URL, enter API key and hash. Save, upload to server. Now open browser and visit server. If you uploaded index.php and the other files to the /status/ folder on your server, visit http://yourdomain.com/status/.


To-Do
=====

1. If offline, offer option to boot.
2. If online, offer option to reboot or shutdown.
3. Secure folder with .htaccess logins.
~~4. Add a feature to do live updates with jQuery.~~


I used
======

PHP, [SolusVM Client API](http://docs.solusvm.com/client_api), [Twitter Bootstrap](http://twitter.github.io/bootstrap/), [Flatly Bootswatch](http://news.bootswatch.com/post/50569764478/flatly-a-flat-theme-by-jenil-gogari), [jQuery Keymapper Plugin](https://github.com/rafaqueque/jquery-keymapper), and [FlipHost](http://www.fliphost.net/vps.html).


How To Contribute
-----------------------------
1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request


Have A Picture
==============

Here's an "Online" screenshot:
![Pretty Picture](http://i.imgur.com/3p9U6NX.png)


And here's an "Offline" screenshot:
![Another Pretty Picture](http://i.imgur.com/30PGnoS.png)
