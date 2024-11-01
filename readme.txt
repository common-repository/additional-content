=== Additional Content ===
Contributors: keesiemeijer
Tags: post,publish,edit,content,post content,the_content,extra,additional,shortcode,shortcodes
Requires at least: 4.0
Tested up to: 5.4
Stable tag: 1.3.0
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Display additional content before or after post content in single post pages. 

== Description ==

Add additional content on a post per post basis in the edit or publish post screen. The additional content editor can be used with all public post types.

Use this plugin for content that you, for whatever reason, don't want to be included in the post content itself, like [shortcodes](https://keesiemeijer.wordpress.com/2015/05/25/how-to-remove-specific-shortcodes-from-post-content/), or code snippets used by other plugins.

Another benefit of using this plugin is if you want content to be displayed before or after content that is automatically added by other plugins. The [priority parameter](https://wordpress.org/plugins/additional-content/faq/) will let you do just that.

For more information visit the [GitHub repository](https://github.com/keesiemeijer/additional-content).

== Installation ==

= Requirements =
[PHP](https://secure.php.net/) 5.4.0 or higher

**Note**: This plugin displays an admin notice when activated on lower PHP versions. Disable this plugin like you normally would in the wp-admin if you see this notice.

**What is PHP?**  
PHP is the scripting language used to build WordPress. It's installed on your server by your host. The [minimum required version](https://wordpress.org/about/requirements/) for WordPress is PHP 5.2.4. This version has been unsupported since early 2011 and is potentially insecure. WordPress supports it to maintain backward compatibility for sites that are still using it.

This plugin is also build with PHP but it requires the PHP version of 5.4.0 or higher to work.

Follow these instructions to install the plugin.
  
1. In your WordPress admin panel, go to Plugins > New Plugin, search for "additional content" and click "Install now".
2. Alternatively, download the plugin and upload the contents of additional-content.zip to your plugins directory, which usually is /wp-content/plugins/.
3. Activate the plugin
4. Add additional content in the edit or publish post screens.

== Frequently Asked Questions ==

= What is the priority option? =
This plugin is basically a user interface for [the_content filter](https://codex.wordpress.org/Plugin_API/Filter_Reference/the_content). This filter allows themes and plugins to change (or add content to) post content before it's displayed. The default priority for filters is 10. Higher numbers correspond with later execution of adding additional content. This option allows you to display the additional content before or after other plugins that add content with this filter.

== Screenshots ==

1. Add additional content in the edit or publish post screen.
2. Additional Content metabox with text strings changed for shortcodes. 
3. Additional Content metabox with options removed with a filter.
4. Warning when activating this plugin on PHP versions smaller than 5.4.0.

== Changelog ==
= 1.3.0 =
* Fix bug where additional content was not displayed in pages. Props: [dpinc](https://profiles.wordpress.org/dpinc).
* Allow unfiltered html for user with the unfiltered_html capability
* Tested up to WordPress 4.6

= 1.2.0 =
* Using anonymous functions for sorting addational content by priority.
* New unit tests
* Tested up to WordPress 4.4

= 1.1.4 =
Initial commit to the WordPress plugins repository.
