How does Chrome-Extension-Downloader work?
Generally
Even Chrome has to connect to a server and download the extension for installing it into your Chrome Browser.

The URL for getting the extension directly is the following:
https://clients2.google.com/service/update2/crx?response=redirect&prodversion=49.0&x=id%3D~~~~%26installsource%3Dondemand%26uc
You have to replace the 4 tildes (~~~~) with the ID of the extension you want to download.

For example if you want to download Google Maps you can find the extension on https://chrome.google.com/webstore/detail/google-maps/lneaknkopdijkpnocmklfnjbeapigfbh.
The extracted ID of Google Maps is lneaknkopdijkpnocmklfnjbeapigfbh.
The direct download URL for Google Maps will be https://clients2.google.com/service/update2/crx?response=redirect&prodversion=49.0&x=id%3Dlneaknkopdijkpnocmklfnjbeapigfbh%26installsource%3Dondemand%26uc.

The downloaded file will always be named as extension_[version].crx.
In our example with Google Maps it is extension_5_2_7.crx, because the current version of Google Maps is 5.2.7.

What is Chrome-Extension-Downloader doing?
Check if it's a valid Chrome Web Store url
Parse the ID of the given URL
Check if the given ID is valid
Parse the name of the extension from Chrome Web Store
Send the extension file with corrected filename directly to you.

