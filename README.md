ownCloud for YunoHost
---------------------

[ownCloud](https://owncloud.org) gives you freedom and control over your
own data. A personal cloud which run on your own server. With owncloud
you can synchronize your files over your devices.

**Shipped version:** 9.0.4

![](https://github.com/owncloud/screenshots/blob/master/files/sidebar_1.png)

## Features

In addition to ownCloud core features, the following are made available with
this package:

 * Integrate with YunoHost users and SSO - i.e. logout button
 * Allow one user to be the administrator (set at the installation)
 * Optionally access the user home folder from ownCloud files (set at the installation)
 * Serve `/.well-known` paths for CalDAV and CardDAV on the domain only if it's
   not already served - i.e. by Baïkal

## Limitations

To integrate the logout button to the SSO, we have to patch ownCloud sources.
Since this upstream [pull-request](https://github.com/owncloud/core/pull/24642)
will not be integrated, the code source integrity checking has been disabled to
prevent the warning message.

Also, note we made the choice to disable third-parties applications at the
upgrade. It allows to prevent an unstable - and sometimes broken - ownCloud
installation. You will just have to manually activate them after the upgrade.

## Links

 * Report a bug: https://dev.yunohost.org/projects/apps/issues
 * ownCloud website: https://owncloud.org/
 * YunoHost website: https://yunohost.org/
