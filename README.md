AlphaLemon CMS Sandbox
======================
Welcome to the AlphaLemon CMS Sandbox - a fully-functional Symfony2
application, powered by AlphaLemon CMS, that you can use as the skeleton
for your new app.

This document contains information on how to download and start using AlphaLemon CMS.

[![Build Status](https://secure.travis-ci.org/alphalemon/AlphaLemonCmsSandbox.png)](http://travis-ci.org/alphalemon/AlphaLemonCmsSandbox)


Download
--------
From your console run the following command:

    git clone https://github.com/alphalemon/AlphaLemonCmsSandbox.git


Permissions
-----------
Setup the permissions on the installation folder as explained in the [symfony2 setup and configuration
tutorial](http://symfony.com/doc/current/book/installation.html#configuration-and-setup)


Vendor libraries installation
-----------------------------

> This step is required only if you are using the "without vendors" sandbox

Once you've downloaded and uncompressed the AlphaLemon CMS Sandbox, just open a console,
move to the root folder and give the following command to download composer and install
the required vendor libraries:

    curl -s http://getcomposer.org/installer | php
    php composer.phar install


AlphaLemon CMS setup
--------------------
AlphaLemonCMS requires several steps to be accomplished to properly setup the CMS itself. Luckily
the **AlphaLemonCmsInstallerBundle** will do all the job for you, providing a web installer interface
or an interactive symdony2 command to install AlphaLemonCMS.


Installing from the console
---------------------------
Installing AlphaLemonCMS from the console is really easy:

    app/console alphalemon:install-cms

This will run the interactive command. Provide the required information and you are done! Point
your browser at

    http://localhost/alcms.php/backend/login

to start using AlphaLemonCMS.


Installing using the web interface
----------------------------------
To Install AlphaLemonCMS using the web interface, just point your browser at:

    http://localhost/app_dev.php/install

Provide the required information and you are done! 


Signin
------
AlphaLemonCms is secured by default and a new user is created when the application is installed:

    username: admin
    password: admin

enter the credentials above to signin.


Documentation
-------------
You can read AlphaLemon CMS official documentation at alphalemon.com:

- [The book](http://alphalemon.com/the-official-alphalemon-cms-documentation)
- [The cookbook](http://alphalemon.com/alphalemon-cms-cookbook)
- [Developers guide](http://alphalemon.com/getting-started-contributing-to-alphalemon-cms)

AlphaLemon CMS [documentation repository](https://github.com/alphalemon/alphalemon-docs)
lives at github.


Support
-------
If you require support you can ask for help at [AlphaLemon CSM users forum](https://groups.google.com/forum/?hl=it#!forum/alphalemoncms-users).

If you want to collaborate, just introduce yourself at [AlphaLemon CSM developers forum](https://groups.google.com/forum/?hl=it#!forum/alphalemoncms-dev).


Stay in touch
-------------
AlphaLemon CMS is present on major social networks:

Follow [@alphalemoncms on Twitter](https://twitter.com/alphalemoncms) for the latest news

Like AlphaLemon CMS at [Facebook](https://www.facebook.com/alphalemon)

Connect with AlphaLemon CMS at [Google+](https://plus.google.com/103994964006724386514/posts)


Notes for windows users
-----------------------
AlphaLemon CMS has been written on a linux system machine, so you might encounter some small issues when
you work on a windows machine:

- assetic:dump command might return an error
- Skin problems

None of those problems breaks the usability of AlphaLemon CMS. If you are a windows user and you want
to fix them on your own, fork the repository, do the fixes then ask for a pull request: it would be really
appreciated! :)

Enjoy!
