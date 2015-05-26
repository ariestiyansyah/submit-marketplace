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
	>
	> If you haven't done so already, you'll be asked to agree to the Firefox Marketplace Developer Agreement. 
	>
	> In this section you can use Firefox Account to register or sign to Firefox Marketplace Hub

#### Step 2 - Step 2 - Load your app
On the Submit an app page:
1. Select whether the app is free or paid.
2. Select the platforms the app will be available on.
3. Select whether the app is hosted or packaged then:

	> For a hosted app, provide the link to its manifest file.
	>
	> For a packaged app, upload the package.zip file, and once it has been validated, identify the minimum API requirements.
4. Click Continue.

#### Step 3 - Enter your app's details
On the Edit App Details page:

1. Modify the app URL if you wish.
2. Modify the description (provided in the manifest) if you wish.
3. Select one or two categories.
4. Provide a Privacy Policy.
5. Defined a home page and support website if you have them.
6. Provide a support email address.
7. Indicate whether the app requires Flash support.
8. Add at least one screenshot or video.
9. Provide additional comments for the app reviewer (such as sign in details if the app requires them) - note you'll only be able to modify these notes by submitting a new version of the app.
10. Select whether the app will be published as soon as approved - note you'll only be able to modify this setting by submitting a new version of the app.
11. Click Continue.

#### Step 4 - See details of the next steps
On the Next Steps page click Continue.

#### Step 5 - Obtain a content rating
On the Content Ratings page:

* to obtain a new rating click Create an IARC Ratings Certificate and on the IARC Web site, complete the ratings questionnaire.
* to enter a rating you've already obtained provide its Submission ID and Security Code.

#### Step 6 - Update availability and payment details
Step 6a - If the app is free (and doesn't include in-app purchases):

* On the left hand menu, click Compatibility. Change the countries the app will be available in if you wish.

Step 6b - If the app is paid (or free, but includes in app payments):

* On the left hand menu, click Compatibility & Payments
	- Setup your payment provider accounts, such as Bango and Boku.
	- Set the price, identify whether the app includes in-app products and select the countries the app will be available in.
	- If the app is being offered as a premium upgrade to a free app, identify the free app.

Step 6c - If the app includes in-app products:

* On the left hand menu click In-App Payments and obtain your API key and secret. (Note that you'll have to submit an update to your app once the API key and secret have been added to it, for more details see In-app payments.)
* If you're using fxPay, on the left hand menu click In-App Products and define each of your in-app products.

#### Step 7 - Setup team member (optional)

* On the left hand menu, click Team Members and add any additional team member if you wish.

#### Step 8 - View the listing (optional)
* On the left hand menu, click View Listing and view your app's Marketplace listing if you wish.

#### Step 9 - Edit other localization listings (optional)

* On the left hand menu click Edit Listing and modify the app URL, description, and categories for any of the app's localizations or add details for any other locale supported by Firefox Marketplace.

Application is now in the review queue. You can monitor its progress through the review process by clicking Status and Version on the left hand menu. Remember that if your app makes use of in-app payments you will need to code in the API Key and submit an update before the app can be published.
