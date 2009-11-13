=== Plugin Name ===
Contributors: phkcorp2005
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=9674139
Tags: https-to-http, https, http, redirection, mavis
Requires at least: 2.8.6
Tested up to: 2.8.6

Provides page redirection back to non-secured pages (https: to http:)

== Description ==

This plugin was developed to solve a redirection issue when navigating from a secured checkout page back to
a non-secured page (or page that you need to have as non-secured---possibly because of external non-secured
external links, etc.)

For example, a user comes to your wordpress e-commerce site, locates an item, then navigates to your
secured checkout page. Now the customer, realizes there is something else they need, and instead of clicking
the Continue Shopping link, they click another category link. Since the customer is in a secured session, wordpress
attached the secured protocol on all the links including that category link the customer is now clicking. 
The customer then navigates to that category page, but they are viewing the page in a secured session. 
This category page is not displaying the elements properly because some external links did not translate 
into the secured session. The customer is now upset, thinking that the site design demonstrates the 
level of incompetence of the shop owner and questions the shop owner's 
integrity to fulfill their order, so the customer in a behavior of discuss, rapidly leaves the
shop owner's site and that customer becomes a non-customer!

This plugin resolves this issue by redirecting all non-specified secured (or other secured pages)
back to a non-secured page counterpart.


== Installation ==

To instal this plugin, follow these steps:

1. Download the plugin mavis.zip
2. Extract the single file mavis.php
3. Upload to the `/wp-content/plugins/` directory
4. Activate the plugin through the 'Plugins' menu in WordPress
5. Change your site to use pretty permalinks from the 'Permalinks' menu in WordPress
6. Set your secured page on the Mavis HTTPS/HTTP Redirection admin page from the 'Settings' menu in Wordpress

== Frequently Asked Questions ==

= Do I need to add any code to my template file, post or pages? =

No. You just specify a unique tag from the permalink of page or parent page that 
will use a secured session.

= Do I need to use permalinks? =

Recommended for better matching.


== Screenshots ==

screenshot-1.png

== Changelog ==

= 1.0 =
* Created
