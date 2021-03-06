# Ampache for YunoHost

[![Integration level](https://dash.yunohost.org/integration/ampache.svg)](https://ci-apps.yunohost.org/jenkins/job/ampache%20%28Official%29/lastBuild/consoleFull)  
[![Install Ampache with YunoHost](https://install-app.yunohost.org/install-with-yunohost.png)](https://install-app.yunohost.org/?app=ampache)

> *This package allow you to install ampache quickly and simply on a YunoHost server.  
If you don't have YunoHost, please see [here](https://yunohost.org/#/install) to know how to install and enjoy it.*

## Overview
[Ampache](http://ampache.org) for the love of music. A web based audio/video 
streaming application and file manager allowing you to access your 
music & videos from anywhere, using almost any internet enabled device.

**Shipped version:** 3.8.6

## Screenshots

![](http://ampache.org/img/previews/visualizer.jpg)

## Configuration

## Documentation

 * Official documentation: 
 * YunoHost documentation: There no other documentations, feel free to contribute.

## YunoHost specific features

In addition to Ampache core features, the following are made available with
this package:

 * Config for high quality streaming with high bandwith
 * Quick loading for mobile devices with potential low bandwith
 * Integrate with YunoHost users - same username and password
 * Allow one user to be the administrator (set at the installation)

#### Multi-users support

 * Ampache is connect to Yunohost LDAP
 * No auto SSO yet

#### Supported architectures

* Tested on x86_64
* Tested on armhf

## Limitations

* The user panel button was disabled because it hides an essential part of the ampache user interface.
* Also, the SSO authentication not fully working from user panel, we have to work about this.
In fact, it can disrupt external Ampache clients like Subsonic.

## Additionnal informations
### Getting started

 * **Add your first catalog to load music files**
   * Go to *Admin panel* ![](https://raw.githubusercontent.com/ampache/ampache/develop/themes/reborn/images/icons/icon_admin.png)
   * Click on *Add a Catalog*
   * Fill up fields and click *Add Calalog*
   * Next, enjoy :)

 * **Update a catalog for load new music files**
   * Go to *Admin panel* ![](https://raw.githubusercontent.com/ampache/ampache/develop/themes/reborn/images/icons/icon_admin.png)
   * Click on *Show Catalogs*
   * Select *Update* in *Actions* list and click *Go*

 * **Change interface Language**
   * Go to *Preferences panel* ![](https://raw.githubusercontent.com/ampache/ampache/develop/themes/reborn/images/icons/icon_edit.png)
   * Click on *Interface*
   * Change *Language* field

### Ampache on mobile devices

 * [For Android](https://play.google.com/store/apps/details?id=com.antoniotari.reactiveampacheapp)
 * [For iOS](http://iampache.com/)

 * Full list of existings clients : https://github.com/ampache/ampache/wiki/Clients

## Links

 * Report a bug: https://github.com/YunoHost-Apps/ampache_ynh/issues
 * Ampache website: http://ampache.org/
 * YunoHost website: https://yunohost.org/

---

Developers infos
----------------

Please do your pull request to the [testing branch](https://github.com/YunoHost-Apps/ampache_ynh/tree/testing).

To try the testing branch, please proceed like that.
```
sudo yunohost app install https://github.com/YunoHost-Apps/ampache_ynh/tree/testing --verbose
or
sudo yunohost app upgrade ampache -u https://github.com/YunoHost-Apps/ampache_ynh/tree/testing --verbose
```
