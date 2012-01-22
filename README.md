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

    php ./bin/vendors install

Now you must grab ElFinder vendor library, which is a submodule of ElFinderBundle. Give
this commands:

    cd vendor/bundles/AlphaLemon/ElFinderBundle/
    git submodule init
    git submodule update

Wait that until the library is downloaded then return to the top directory. 

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

    php ./bin/cmsInstall

Use AlphaLemon CMS
------------------

To browse your site, simply open a browser and point to http://localhost or whatever your domain is.

To work with AlphaLemon CMS simply point to http://localhost/alcms.php/en/index. You may debug your
application using the alcms_dev.php environment: http://localhost/alcms_dev.php/en/index

Enjoy!
