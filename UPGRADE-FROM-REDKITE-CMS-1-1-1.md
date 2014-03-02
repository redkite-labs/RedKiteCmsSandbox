Upgrade from RedKite CMS 1.1.1
==============================

This release comes with several third-party libraries upgraded, in particular
Twitter Bootstrap has been updated to latest release.

In additional, Font-Awesome library has been added and it is required to properly
render the new RedKite CMS interface.


Upgrade
-------

To upgrade your RedKite CMS application you must update those libraries using
bower as explained here: http://redkite-labs.com/how-to-install-redkite-cms#install-assets.

If you don't want to deal with bower, just download the new RedKite CMS Sandbox and
replace the web/components folder of your application, with the one that comes with
the downloaded sandbox.

When you completed that task, clear the cache and run those commands:

    php app/console ca:c --env=rkcms
    php app/console assetic:dump --env=rkcms


Upgrade your themes
-------------------

This release does not come with yuicompressor anymore to let people choose the preferred compressor
to minify assets.

Due to that change, the filter="?yui_*" option must be removed from templates and must be replaced
as explained in the Symfony2 cockbook http://symfony.com/doc/current/cookbook/assetic/apply_to_option.html#filtering-based-on-a-file-extension.

Please note that the enable_yui_compressor parameter has been removed.
