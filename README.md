RedKite CMS Sandbox
====================
Welcome to RedKite CMS Sandbox - a fully-functional Symfony2 application
powered by RedKite CMS. You can use this application as skeleton for 
your new project or to test the CMS itself.

This document contains information on how to download and to start using 
RedKite CMS.

[![Build Status](https://secure.travis-ci.org/redkite-labs/RedKiteCmsSandbox.png)](http://travis-ci.org/redkite-labs/RedKiteCmsSandbox)


Download
--------
From your console run the following command:

    git clone https://github.com/redkite-labs/RedKiteCmsSandbox.git


Permissions
-----------
Setup the permissions on the installation folder as explained in the [symfony2 setup and configuration
tutorial](http://symfony.com/doc/current/book/installation.html#configuration-and-setup)


Vendor libraries installation
-----------------------------

> This step is required only if you are using the "without vendors" sandbox

Once you've downloaded and uncompressed RedKite CMS Sandbox, just open a console,
move to the root folder and give the following command to download composer and install
the required vendor libraries:

    curl -s http://getcomposer.org/installer | php
    php composer.phar install


RedKite CMS setup
-----------------
RedKite CMS requires several steps to be accomplished to properly setup the CMS itself. Luckily
the **RedKiteCmsInstallerBundle** will do all the job for you. 

This bundle provides a web installer interface or an interactive symdony2 command to install 
RedKite CMS.

Installing from the console
---------------------------
Installing RedKite CMS from the console is really easy:

    app/console rekitecms:install

This will run the interactive command. Simply provide the required information and you are done! 

When the setup ends, point your browser at

    http://localhost/rkcms.php/backend/login

to start using RedKite CMS.


Installing using the web interface
----------------------------------
To install RedKite CMS using the web interface, just point your browser at:

    http://localhost/app_dev.php/install

Provide the required information and you are done! 


Sign in
-------
RedKite CMS is secured by default and a new user is created when the application is 
installed:

    username: admin
    password: admin

enter the credentials above to sign in.


Documentation
-------------
Although RedKite CMS is designed to be as simple and intuitive as possible, you probably 
would like to go deeper reading some documentation:

- [The book](http://redkite-labs.com/getting-started-with-redkite-cms)
- [The cookbook](http://redkite-labs.com/redkite-cms-practical-manual-part-1)
- [Developers guide](http://redkite-labs.com/getting-started-contributing-to-redkite-cms)

RedKite CMS [documentation repository](https://github.com/redkite-labs/redkitecms-docs)
lives at github.


Support
-------
If you require support you can ask for help at [RedKite CSM users forum](https://groups.google.com/forum/?hl=it#!forum/redkitecms-users).

If you want to collaborate, just introduce yourself at [RedKite CSM developers forum](https://groups.google.com/forum/?hl=it#!forum/redkitecms-dev).


Stay in touch
-------------
RedKite CMS is present on major social networks:

Follow [@redkite-cms on Twitter](https://twitter.com/redkitecms) for the latest news

Like RedKite CMS at [Facebook](https://www.facebook.com/redkitecms)

Connect with RedKite CMS at [Google+](https://plus.google.com/103994964006724386514)


Notes for windows users
-----------------------
RedKite CMS has been written on a linux system machine, so you might encounter some small issues when
you work on a windows machine:

- assetic:dump command might return an error
- Skin problems

None of those problems breaks the usability of RedKite CMS. If you are a windows user and you want
to fix them on your own, fork the repository, do the fixes then ask for a pull request: it would be really
appreciated! :)

Enjoy!
