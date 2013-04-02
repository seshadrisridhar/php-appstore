php-appstore
===================

PHP class with a bunch of functions to retrieve app details, ratings, reviews and rankings from the App Store

Questions/Comments? Follow me on Twitter <a href="http://twitter.com/albeebe">@albeebe</a>

<h1>Uses </h1>

Armed with nothing more then an App ID, you can pull a ton of information about the app from the App Store.  Reviews, ratings, app details, ranking information and more!

<h1>Example.php </h1>

<PRE>
include ("appstore.inc.php");

$appID = "577499909"; // Angry Birds

$_APPSTORE = new APPSTORE($appID);
$arrReviews = $_APPSTORE->reviewsForPage(0);
$appName = $_APPSTORE->appName();
$appIcon = $_APPSTORE->appIcon();
$appDeveloper = $_APPSTORE->appDeveloper();
$appTotalStars = $_APPSTORE->appTotalStars();
$appTotalRatings = $_APPSTORE->appTotalRatings();
$appCurrentStars = $_APPSTORE->appCurrentStars();
$appCurrentRatings = $_APPSTORE->appCurrentRatings();
$appCategoryName = $_APPSTORE->appCategoryName();
$appCategoryID = $_APPSTORE->appCategoryID();
$appRankCategory = $_APPSTORE->appRankCategory();
$appRankCategoryGrossing = $_APPSTORE->appRankCategoryGrossing();
</PRE>

Here is a screenshot of example.php running on an iPhone, with Angry Birds set as the appID

<IMG STYLE="border:1px solid black" SRC="http://i48.tinypic.com/124zj8w.png" WIDTH="320" HEIGHT="568">

<h1>License</h1>
The MIT License
<BR>
<BR>Copyright (c) 2013 Alan Beebe
<BR>
<BR>Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
<BR>
<BR>The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
<BR>
<BR>THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.