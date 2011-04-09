=== Mavis HTTPS to HTTP Redirection ===
Contributors: phkcorp2005
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=9674139
Tags: https-to-http, https, http, redirection, mavis
Requires at least: 2.9
Tested up to: 2.9
Stable tag: 1.4.1

Provides page redirection back to non-secured pages (https: to http:)

== Description ==

This plugin was developed to solve a redirection issue when navigating from a secured checkout page back to
a non-secured page (or page that you need to have as non-secured---possibly because of non-secured
external links, etc.)

For example, a user comes to your wordpress e-commerce site, locates an item, then navigates to your
secured checkout page. Now the customer, realizes there is something else they need, and instead of clicking
a Continue Shopping link, then click a top category link. Since the customer is in a secured session, wordpress
put the secured protocol on all the links including that category. Now the customer navigates to that
category, but they are still in a secured page session. Now this category page is displaying improperly because
of some external links that did not translate properly into the secured session. Customer is now upset, thinking
that the site design demonstrates the level of incompetence of the shop owner and questions the shop owner's 
integrity to fulfill the customer's order, so the customer in a behavior of discuss, rapidly leaves the
shop owner's site and that customer becomes a non-customer!

This plugin resolves this issue by redirecting all non specified checkout (and other non-secured pages)
back to a non-secured page counterpart.


== Installation ==

To instal this plugin, follow these steps:

1. Download the plugin mavis.zip
2. Extract the single file mavis.php
3. Extract mavis plugin to the `/wp-content/plugins/` directory as new directory will be created identified as 'mavis-https-to-http-redirect'
4. Activate the plugin through the 'Plugins' menu in WordPress, identified by 'Mavis HTTPS to HTTP Redirection'
5. Change your site to use pretty permalinks from the 'Permalinks' menu in WordPress
6. Set your secured page on the 'Mavis HTTPS/HTTP Redirection' admin page from the 'Settings' menu in Wordpress
7. If you have more than one secured page, separate each page name using commas (e.g. checkout,confirm)

== Frequently Asked Questions ==

Please do not be afraid of asking questions?<br>

(There are no stupid or dumb questions!)


== Changelog ==
= 1.4.1 =
* Fix a bug that prevented displaying secured page list in text field properly

= 1.4 =
* Fix a bug that prevented plugin from being activated when php short definition is not defined.

= 1.3 =
* Filtered code from NOT being executed during an admin session. Apparently, one user reported that it does?

= 1.2 =
* Added support for multiple secured page checking
* Forced redirect of secure page tags back to a secured page session if session is unsecured

= 1.0 =
* Created

== Upgrade Notice ==
= 1.4.1 =
See 1.4 upgrade notice

= 1.4 =
If your server has not enabled short php definitions, then you must upgrade to this version

= 1.3 =
Apparently the redirection is executed during an admin session as a user had reported. The change includes a filter to prevent the plugin from redirecting during an admin session

= 1.2 =
Adds support for permitting more than one secured page to be checked. This is a user-requested feature, as the user reported that certain ecommerce plugins had a second secured page that was getting redirected back to an unsecured session.

== Credits ==

We make honorable mention to anyone who helps make Mavis HTTPS to HTTP Redirect a better plugin!

== Contact ==

For support, go to http://support.phkcorp.com and request to join the "Mavis HTTPS to HTTP Redirection" forum.

Please contact phkcorp2005@gmail.com or visit www.phkcorp.com?do=wordpress with questions, comments, or requests.
