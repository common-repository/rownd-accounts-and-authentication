=== Rownd — Instant user accounts and authentication ===
Contributors: rownd, mhamann
Tags: users, authentication, accounts, profile, woocommerce, auth, login, social login, register, signin, oauth, authorize
Requires at least: 4.5
Tested up to: 6.6
Requires PHP: 7.2
Stable tag: 1.3.4
License: Apache 2.0
License URI: http://www.apache.org/licenses/LICENSE-2.0

Instantly turn visitors into users with Rownd's radically simple, user-centric authentication.

== Description ==

Rownd is a user authentication and account platform that helps you convert more visitors to your website into actual (paying) customers.

We're focused on passwordless sign-in that uses email and SMS as a means of distributing authentication links that allow users to verify
their email/phone after they've had the opportunity to explore your product or service.

When you install the Rownd plugin for WordPress, you'll bring our powerfully simple authentication and user account capabilities into
your website, blog, or ecommerce site.

Rownd integrates with the existing WordPress user management system, which means we're compatible with WooCommerce and many other
WordPress addons! We'll also detect whether you have WooCommerce installed and provide options to customize your customer experience
during the checkout process.

Whether you're accepting user signups already or want to start, Rownd makes it super-simple to get visitors and customers up and running quickly.
Easily trigger our sign-in dialog by setting some HTML data attributes in your code or writing some simple Javascript and we'll handle getting
your users verified and signed in using our unique, passwordless approach.

To get started, you'll need:

1. A free [Rownd account](https://app.rownd.io)
2. A Rownd app key

Once you install this plugin, drop your app key and secret into our settings and you'll be good to go!

Usage of this plugin is governed by Rownd's [terms of service](https://rownd.io/terms-and-conditions).

== Installation ==

**Automated installation**
Installation is free, quick, and easy. Just hit the "Install Now" button, activate the plugin, and add your Rownd app key and secret.

Manual alternatives
Alternatively, install Rownd via the plugin directory, or upload the files manually to your server's `wp-content/plugins` directory.
If you need additional help [read our documentation.](https://docs.rownd.io/)

== Screenshots ==

1. Rownd allows visitors to sign in simply via UX components, which you can also trigger from any HTML page element.
2. Once authenticated, users can manage their accounts from any page on the site.
3. Manage your Rownd integration easily through our simple settings pane.

== Changelog ==

= 1.3.4 =
* Fix: Rownd-initiated API calls now take permalink configuration into account

= 1.3.4 =
* Feature: Delay the Rownd sign-in dialog until after showing the order details

= 1.3.2 =
* Fix: Auto-submit the Rownd sign-in dialog after passing the order email address

= 1.3.1 =
* Fix: WooCommerce customers created in the after-checkout process were not updated with their last order data
* Fix: When sign-in was triggered before the checkout process, it was attempting to access an order property from a checkout object

= 1.3.0 =
* Feature: Improves loading time for Rownd components via support for JavaScript Modules (ESM)

= 1.2.5 =
* Fix: Rownd and WordPress users could become cross-contaminated in the local browser if the current WP session didn't get invalidated during sign out and another user signed into the same browser immediately thereafter.

= 1.2.4 =
* Fix: Rownd IDs were not added to user meta when signed in by WooCommerce after checkout
* Fix: Login links within a WooCommerce checkout flow reverted to the standard WC login form

= 1.2.3 =
* Fix: Rownd IDs were not added to user meta for existing users
* Fix: Anonymous user ID might be set when calling the WP/WC REST API without a Rownd token
* Feature: Support fetching users via Rownd ID in the WP and WC REST APIs

= 1.2.2 =
* Fix: a bug in the `profile_update` hook could cause order failures during the WooCommerce checkout process
* Fix: the setting specifying where a user should sign in during a WooCommerce checkout flow did not reflect properly in the admin page
* Feature: pass order email address to the Rownd sign-in dialog after WooCommerce order creation

= 1.2.1 =
* Fix: Improved error handling in certain situations

= 1.2.0 =
* Feature: Require sign-in during or after the WooCommerce checkout process
* Feature: Replace WooCommerce authentication functions
* Fix: Page refresh loop due to certain circumstances that prevented session initialization

= 1.1.2 =
* Fix: Asset caching was not using the plugin version as the cache key

= 1.1.1 =
* Fix: Changes to API endpoint settings were not honored

= 1.1.0 =
* Feature: Admins may set root origin for use across multiple sites
* Feature: Admins may disable management of WordPress users when someone authenticates (defaults to enabled).

= 1.0.0 =
* Initial release

== Upgrade Notice ==

= 1.3.4 =
Upgrade for minor fixes to REST API interfaces

= 1.3.4 =
Upgrade for performance improvements

= 1.3.2 =
Upgrade for minor bug fixes affecting WooCommerce checkout flows

= 1.3.1 =
Upgrade for critical bug fixes affecting WooCommerce checkout flows

= 1.3.0 =
Upgrade for performance improvements

= 1.2.5 =
Upgrade for minor bug fixes

= 1.2.4 =
Upgrade for minor bug fixes affecting WooCommerce checkout flows

= 1.2.3 =
Upgrade for critical bug fixes

= 1.2.2 =
Upgrade for critical bug fixes affecting Rownd integration and WooCommerce checkout.

= 1.2.1 =
Upgrade for critical bug fixes and to enable deeper integration with WooCommerce!

= 1.1.2=
Upgrade for critical bug fixes

= 1.1.0 =
Upgrade to enable finer control of Rownd's WordPress integration.

= 1.0.0 =
Install our initial release!
