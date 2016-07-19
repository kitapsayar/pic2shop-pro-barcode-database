Pic2shop-pro-barcode-database
=============================

Single-file PHP database that integrates with mobile barcode scanner app *pic2shop® PRO* (Android and iOS).

**This is not a barcode scanner.** This code demonstrates how to use pic2shop PRO to build a barcode-enabled online database.

About pic2shop PRO
------------------

**Pic2shop PRO** is a paid app available for iOS and Android.  It reads EAN13, EAN8, UPC-A, UPC-E, Code 39, Code 93, Code 128, ITF (Interleaved 2 of 5), Standard 2 of 5 (aka Code 25 or Ind2of5) and Codabar (aka USD-4, NW-7) barcodes. After each scan, the app displays a user-defined url with the barcode string as parameter in the embedded web browser. EAN and UPC codes can be read with fixed-focus cameras, such as the iPod Touch 4th gen, the iPad2, the iPad front camera and many Android devices.

[Pic2shop PRO] [1] is developed by [Vision Smarts] [2].

Functionalities
---------------

The purpose of this sample code is to demonstrate how to integrate a web app with the mobile app pic2shop PRO. It uses PHP and SQLite but the same results can easily be achieved with other web frameworks.

Automatic app configuration link (formats, Home page, Lookup page) via: 
	
	p2spro://configure?

Start a scan from a link in the page (with the option to override the lookup target) via:

	p2spro://scan?

Insert barcode data into a field via a javascript callback:

	p2spro://scan?callback=javascript:insertCodeFormat()

Image upload via:

	<input type="file" accept="image/*" capture="camera" name="image">

Retrieve GET parameters when the Home or Lookup URLs are fetched.

Retrieve POST parameters when the form is submitted.

Suggestions for extensions
--------------------------

In real settings, a number of improvements would be needed:

* Replace SQLite with MySQL or PostgreSQL
* Organize the code in separate files (css, js, html view, php model+controller, etc)
* Add a style sheet
* Add better data validation
* Add user authentication

Trademarks
----------

IPHONE, IPOD and IPAD are trademarks of Apple Inc., registered in the U.S. and other countries. 
IOS is a trademark or registered trademark of Cisco in the U.S. and other countries. 
ANDROID is a trademark of Google Inc. 


[1]: http://www.pic2shop.com/pro_version.html "pic2shop PRO"
[2]: http://www.visionsmarts.com              "Vision Smarts"


[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/VisionSmarts/pic2shop-pro-barcode-database/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

