# Embedding SSH tours in your website

## Overview
The Smart Show Home (SSH) 360 Tour is a custom built web application hosted on our SSH server and managed by ‘Client Manager’ integral CMS. Tours can be hosted on multiple websites at the same time via iframe. ie: Client website, Estate Agent website and marketplace websites like Rightmove and Zoopla.

The tour also has a PWA version and can be saved to home screen.

Changes within tours made via Client Manager, such as price and description changes, are dynamically updated and can be viewed live. In some instances you may need to refresh the browser to view updates. Software version updates containing new features or bug fixes are all managed at SSH HQ and are also dynamically updated.

SSH contains cookies to personalise the user experience and app performance. We do not share user information with 3rd parties. 

SSH has an integral viral engine called Social Media Marketing (SMM)  which enables the Client to generate advert posts directly from Client Manager on social media platforms like facebook and Twitter. Also within the tours users can share their favourite houses with friends and family. These posts in turn allow new users to onboard directly from social media platforms. To generate these posts and shares SSH requires a folder containing relevant image files to be hosted on the domain and code to be embedded within the web page. 

## Hosting tour on a website
There are 2 steps to host a SSH tour on a domain:

 1. add iframe
 2. set iframe options

### Add iframe

Iframe tag should be created within page HTML code. Make sure it will be able to take 100% of page width excluding left and right screen margins. Iframe block requires a title before it. The title may be 'Virtual Show Home'.

### Iframe options
Iframe tag should have the following parameters:

 - width: 100%;
 - height: recommended setting is 700px for desktops and tablets in landscape orientation;
 - `allowfullscreen`. The tour has option to go fullscreen;
 - `id="tour"`. The tour needs unique id for correct functioning of all features

For mobiles there are two options:
* provide a a direct link to the tour, so user will get fullscreen version;
* embed tour via iframe with height about 300px and width to 100% of device screen. The tour will recognise it's state and will offer user to open fullscreen version in new tab *(in development)* 

### Iframe URL
 
 Iframe URL is provided by SSH and looks like this:

   https://developer.smartshowhome.com/development/pagelink=https://developer.smartshowhome.com&iframeId=10

Link parameters:
* `pagelihk` is a link to redirection page which provides correct data for social media sharing and leads users to development webpage when clicked.
* `iframeId` - SSH internal page id.

If you need more places to embed the tour please contact SSH.
