Submitting Application to Marketplace Content Kit
=================================================

Introduction
------------

Firefox Marketplace is ecosystem for the Open Web Application. The Applications
are not just restricted to Firefox OS Mobile Application but they also cater of
Firefox Browser Add-ons, Firefox for Androis apps, etc. Using standard Web
technologies, languages, and tools, the [Firefox
Marketplace](http://marketplace.firefox.com) enables you to publish free and
paid Apps. These apps can be packaged, running within Firefox, or hosted on
your own web server.

Key Points
----------

1. Learn and How-To submit application to Firefox Marketplace.
2. Application publishing overview.
3. Currently submission support for Firefox OS, Firefox OS Tablet, Desktop, Firefox for Android. 
4. Firefox Marketplace  is a unified marketplace for applications in the
   Firefox Ecosystem (Apps, Add-ons, Firefox for Android, Firefox OS Apps), so
you need to tell what kind of App you are submitting.
5. Hosting and Packages application.

Reference Materials
-------------------

Firefox Marketplace:

* Landing: https://marketplace.firefox.com/developers/submit/
* Docs:
  https://developer.mozilla.org/en-US/Marketplace/Publishing/Submit/Overview


Firefox Account: 
* Landing: https://accounts.firefox.com/
* Wiki: https://wiki.mozilla.org/Identity/Firefox_Accounts
* MDN: https://developer.mozilla.org/en-US/docs/Mozilla/Tech/Firefox_Accounts

Presentation Setup and Materials
--------------------------------

For __any presentation__:

- [ ] Browser (Latest Firefox Browser is better)
- [ ] Internet connection for every device in the demo
- [ ] Complete Open Web Application to submit

Demoing: Things that are Broken
-------------------------------

### Manifest

Have a quick look at the app manifest (the 'View' link next to the manifest
url). If the manifest obviously isn't valid JSON/isn't found it won't install
anyway. The [manifest spec](https://developer.mozilla.org/docs/Apps/Manifest) should be consulted if you aren't sure about syntax.
Any issues, reject.

Please take a look at [Serving
manifests](https://developer.mozilla.org/en-US/Apps/Build/Manifest#Serving_manifests) on MDN to served manifest from the [same origin](https://developer.mozilla.org/en-US/Apps/Build/Building_apps_for_Firefox_OS/App_manifest_FAQ#What_is_an_origin.3F)

### AppCache

A common issue on FirefoxOS is 'download halted' during installation - this is
most often due to a broken appcache, either because it doesn't exist. You can
check the manifest at [manifest-validator.com](http://manifest-validator.com/)

### Permissions

Take note of any requested permissions in the manifest. There is a Security
Checklist of available APIs and what they might be used/abused for, as well as
in-depth [Security guidelines for developers and reviewers](https://developer.mozilla.org/en-US/docs/Web/Apps/Security_guidelines). There are only a few
APIs are available to hosted/non-privileged apps (alarms, desktop-notification,
geolocation, fmradio) 

### Icon

* Icons in other sizes, and specified in your app's manifest file, for optimal
  display in other platforms/contexts :
	- A 60 x 60px icon for display on the device.
	- 32 x 32px, 90 x 90px, 120 x 120px, and 256 x 256px icons for optimal display on various other platforms your app can be installed on, such as Windows 7 and Android

Demoing: The Good Parts
-----------------------

### Step by Step Submitting Application

#### Step 1 - Sign in to Developer Account

1. Go to the [Firefox Marketplace Developer
   Hub](https://marketplace.firefox.com/developers/)
2. Click `Submit your app to the Marketplace`
3. Sign in to your developer account
	> If you aren't registered you'll be asked to register.
	> If you haven't done so already, you'll be asked to agree to the Firefox Marketplace Developer Agreement. 
	> In this section you can use Firefox Account to register or sign to Firefox Marketplace Hub

#### Step 2 - 
