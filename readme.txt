=== WC Free Gift Coupons Bulk Coupon Generator ===
Contributors: enginescript
Tags: woocommerce, coupons, bulk, free-gifts, gift-coupons
Requires at least: 6.5
Tested up to: 6.8
Stable tag: 1.2.0
Requires PHP: 7.4
License: GPL v3 or later
License URI: https://www.gnu.org/licenses/gpl-3.0.html

Bulk generate free gift coupons that work with Free Gift Coupons for WooCommerce plugin with proper data structure.

== Description ==

WC Free Gift Coupons Bulk Coupon Generator is a specialized WordPress plugin designed to work specifically with the **Free Gift Coupons for WooCommerce** plugin. It generates bulk free gift coupons with the correct data structure that other coupon generators cannot provide.

**IMPORTANT**: This plugin requires the Free Gift Coupons for WooCommerce plugin to function properly. The Free Gift Coupons plugin can be purchased at https://woocommerce.com/products/free-gift-coupons/

The plugin creates coupons with the proper `gift_info` array structure required by the Free Gift Coupons plugin, ensuring compatibility where other bulk coupon generators fail.

Key features:
* **Free Gift Compatibility**: Specifically designed for Free Gift Coupons for WooCommerce plugin
* **Bulk Generation**: Create up to 100 free gift coupons at once with built-in rate limiting
* **Multi-Product Support**: Select multiple products as free gifts in a single coupon
* **Proper Data Structure**: Creates gift_info arrays with correct product ID mapping
* **Custom Prefixes**: Add custom prefixes to coupon codes for easy organization
* **Security First**: CSRF protection, input sanitization, output escaping, and capability checks
* **User-Friendly Interface**: Clean, responsive admin interface with real-time validation
* **Performance Optimized**: Transient caching, batch processing, and server-friendly delays
* **Internationalization Ready**: Full i18n support with translation files
* **Clean Uninstall**: Removes all plugin data when uninstalled

Perfect for:
* Promotional campaigns with product-specific discounts
* Bulk coupon creation for marketing events
* Educational platforms offering course-specific discounts
* E-commerce stores needing organized coupon management

This plugin is built with security as the top priority, implementing multiple layers of protection against common vulnerabilities while maintaining excellent performance and user experience.

== Installation ==

1. Purchase and install the Free Gift Coupons for WooCommerce plugin from https://woocommerce.com/products/free-gift-coupons/
2. Upload the plugin files to the `/wp-content/plugins/free-gift-bulk-coupon-generator` directory, or install the plugin through the WordPress plugins screen directly.
3. Activate the plugin through the 'Plugins' screen in WordPress.
4. Ensure WooCommerce is installed and activated.
5. Navigate to WooCommerce → Free Gift Bulk Coupons in your WordPress admin.
6. Select products, set the number of coupons, add a custom prefix, and click "Generate Free Gift Coupons".

== Frequently Asked Questions ==

= What are the system requirements? =

* WordPress 6.5 or higher
* WooCommerce plugin installed and activated
* Free Gift Coupons for WooCommerce plugin (required - purchase at https://woocommerce.com/products/free-gift-coupons/)
* PHP 7.4 or higher
* Administrator or Shop Manager capabilities

= How many coupons can I generate at once? =

The plugin allows up to 100 coupons per batch to prevent server timeouts and maintain performance. This limit is enforced both in the UI and server-side validation.

= Can I customize the coupon codes? =

Yes! You can add a custom prefix to all generated coupon codes. For example, using prefix "SUMMER" will generate codes like "SUMMER_ABC123", "SUMMER_DEF456", etc.

= Are the generated coupons secure? =

Absolutely. Each coupon code is generated using WordPress's cryptographically secure wp_generate_password() function, ensuring codes are unpredictable and unique.

= Can I restrict coupons to specific products? =

Yes, you can select one or more products when generating coupons. The generated coupons will only be valid for the selected products.

= What discount type is used for generated coupons? =

The plugin generates free gift coupons that work with the Free Gift Coupons for WooCommerce plugin. These coupons provide free products rather than percentage or fixed amount discounts.

= Is the plugin translation-ready? =

Yes, the plugin includes a .pot file and is fully prepared for translation into any language.

= How do I uninstall the plugin? =

Simply deactivate and delete the plugin through the WordPress admin. The plugin includes a clean uninstall process that removes all its data from your database.

= Can developers extend the plugin? =

Yes! The plugin includes numerous hooks and filters for developers to customize coupon generation, validation, and the admin interface.

== License ==

This plugin is licensed under the GPL v3 or later.

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.

== Changelog ==

= 1.1.0 =
* **Text Domain Standardization**: Fixed WordPress textdomain to match plugin slug for proper internationalization
* **Internationalization Compliance**: Updated all translation functions and POT file to use consistent textdomain
* **Code Quality**: Enhanced code documentation and inline comments for better maintainability  
* **WordPress Standards**: Improved compliance with WordPress coding standards and best practices
* **Coupon Generation**: Restored full character set for coupon codes (all lowercase letters and digits)
* **File Structure**: Renamed POT file to match WordPress naming conventions
* **Security Enhancement**: Additional input validation and sanitization improvements
* **Documentation**: Added comprehensive changelog.txt file for WordPress.org compatibility
* **Technical Improvements**: Updated load_plugin_textdomain(), standardized all translation function calls
* **Developer Experience**: Enhanced PHPDoc comments and improved error logging

= 1.0.0 =
* **Initial Release**: Complete WordPress plugin based on original WooCommerce coupon snippet
* **Security Features**: CSRF protection, input sanitization, output escaping, rate limiting
* **Bulk Generation**: Create up to 100 coupons at once with server-friendly processing
* **Product Selection**: Multi-select dropdown for product-specific coupon restrictions  
* **Custom Prefixes**: Add custom prefixes to organize coupon codes
* **Admin Interface**: Clean, responsive UI with real-time validation and feedback
* **Performance**: Transient caching, batch processing, and optimized database queries
* **Internationalization**: Full i18n support with .pot translation file
* **Developer Friendly**: Extensive hooks and filters for customization
* **Clean Uninstall**: Complete data removal when plugin is deleted
* **Path Validation**: Improved security by validating logical path structure before filesystem operations
* **Attack Surface Reduction**: Minimized potential attack vectors by pre-validating user input before realpath() calls
* **Security Logging**: Enhanced security event logging for better monitoring of potential attacks


== Upgrade Notice ==

= 1.1.0 =
Important update: Fixed WordPress textdomain for proper internationalization. Enhanced code quality and WordPress standards compliance.

= 1.0.0 =
Initial release - Secure bulk free gift coupon generator for WooCommerce with proper Free Gift Coupons plugin compatibility.