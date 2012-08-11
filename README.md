PRE-ALPHA Release
==================================

> This is a Pre-Alpha release. Its pourpose is to let developers to install
it for contributing. It's buggy so don't use it in production.

AlphaLemon CMS Sandbox
======================

Welcome to the AlphaLemon CMS Sandbox - a fully-functional Symfony2
application, powered by AlphaLemon CMS, that you can use as the skeleton
for your new app.

This document contains information on how to download and start using AlphaLemon CMS.

Download
--------

From your console run the following command:

    git clone https://github.com/alphalemon/AlphaLemonCmsSandbox.git


Vendor libraries installation
-----------------------------

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

    http://localhost/alcms.php/backend/en/index

to start using AlphaLemonCMS.

Installing using the web interface
----------------------------------
Installing AlphaLemonCMS using the web interface requires an addictional step, since Symfony 2.1
will be released:

    app/console assets:install web

After the assets have been installed, point your browser at:

    http://localhost/app_dev.php/install

Provide the required information and you are done! After the process ended, you will be immediatly
redirected to the

    http://localhost/alcms.php/backend/en/index

Permissions
-----------
Don't forget to setup the permissions on the installation folder as explained in the [symfony2 setup and configuration
tutorial](http://symfony.com/doc/current/book/installation.html#configuration-and-setup)

Run test suite
--------------
From the root of AlphaLemon CMS Sandbox run the following command:

    phpunit -c app

Stay in touch
-------------
Follow [@alphalemon on twitter](https://twitter.com/alphalemon) for the latest news

Enjoy!
