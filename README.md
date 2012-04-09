AlphaLemon CMS Sandbox
========================

Welcome to the AlphaLemon CMS Sandbox - a fully-functional Symfony2  
application, powered by AlphaLemon CMS, that you can use as the skeleton 
for your new app. 

This document contains information on how to download and start using AlphaLemon CMS.
For a more detailed explanation, see the
[Installation chapter](http://http://alphalemon.com/how-to-install-alphalemon-cms).

Vendor libraries installation
-----------------------------

Once you've downloaded and uncompressed the AlphaLemon CMS Sandbox, just open a console, 
move to the root folder of the sandbox and give the following command to install vendor 
libraries:

    curl -s http://getcomposer.org/installer | php
    php composer.phar update


The bootstrap.php.cache file
----------------------------
AlphaLemonCMS sandbox comes with a precompiled bootstrap.php.cache. If you want to recompile it simply run the
following command:

    php bin/build_bootstrap


AlphaLemon CMS setup
--------------------

Before starting the setup operation, you must configure the parameters required by the application.
The installation script comes with a config.php where are saved the default configurations required 
to install the CMS, which are:

- A bundle where AlphaLemon CMS will save your contents
- The database parameters, like the host, the database name, the user and password

When you start a new Symfony2 project you always create a new bundle where your application lives. 
The required external bundle, by AlphaLemon CMS, is exactly that bundle.

Open the bin/config.php file and change the parameters to work with your environment then give the following 
command to setup AlphaLemon CMS: 

    php vendor/bin/cms-install

Permissions
Don't forget to setup the permissions on the installation folder as explained in the [symfony2 setup and configuration
tutorial](http://symfony.com/doc/current/book/installation.html#configuration-and-setup)

Use AlphaLemon CMS
------------------

To browse your site, simply open a browser and point to **http://localhost** or whatever your domain is.

To work with AlphaLemon CMS simply point to **http://localhost/alcms.php/en/index**. You may debug your
application using the alcms_dev.php environment: **http://localhost/alcms_dev.php/en/index**

Enjoy!
