Skip to content
 This repository
Explore
Gist
Blog
Help
@em57 em57

 Watch 911
  Star 5,310
  Fork 2,652
WordPress/WordPress
 Code
 Pull requests 4
 Pulse
 Graphs
HTTPS clone URL

You can clone with HTTPS, SSH, or Subversion. 

 Clone in Desktop  Download ZIP
WordPress, Git-ified. Synced via SVN every 15 minutes, including branches and tags! This repository is just a mirror of the WordPress subversion repository. Please do not send pull requests. Submit patches to http://core.trac.wordpress.org/ instead. 
http://wordpress.org/
 29,297 commits
 23 branches
 95 releases
 20 contributors
 PHP 69.1%	 JavaScript 16.0%	 CSS 14.3%
PHP	JavaScript	CSS
 branch: master WordPress/ 
TinyMCE: when pasting an URL, check if the node it is pasted at is em… …

latest commit 4bb5d76abc
 Andrew Ozz authored a day ago
wp-admin	Remove leading newlines from two translatable strings.	2 days ago
wp-content	Bundled themes: update editor styles to better display images and cap…	2 days ago
wp-includes	TinyMCE: when pasting an URL, check if the node it is pasted at is em…	a day ago
index.php	Don't rely on include_path to include files.	2 years ago
license.txt	Update license copyright year to 2015.	3 months ago
readme.html	Update readme recommendations. fixes #31173.	2 months ago
wp-activate.php	`wpmu_activate_signup()` returns an `array` or `WP_Error`. The array …	7 months ago
wp-blog-header.php	Lose EOF ?>. Clean up EOF newlines. fixes #12307	3 years ago
wp-comments-post.php	The keyword `elseif` should be used instead of `else if` so that all …	2 months ago
wp-config-sample.php	Remove 'WordPress Language' reference from wp-config-sample.php.	6 months ago
wp-cron.php	Add a missing DocBlock for the core utility function `_get_cron_lock()`.	4 days ago
wp-links-opml.php	Move upgrader_process_complete for core to its proper place in Core_U…	a year ago
wp-load.php	Add inline documentation to clarify the reasoning behind the various …	a month ago
wp-login.php	Introduce a `logout_redirect` filter so the redirect destination can …	a month ago
wp-mail.php	Fix syntax for single- and multi-line comments in root-directory files.	8 months ago
wp-settings.php	Remove obsolete inline comment.	3 months ago
wp-signup.php	Improve the `@param` docs for `trackback_response()` and `validate_an…	4 months ago
wp-trackback.php	Improve the `@param` docs for `trackback_response()` and `validate_an…	4 months ago
xmlrpc.php	Fixes for hooks documentation on xmlrpc.php.	a year ago
 readme.html
<!DOCTYPE html>
<html>
<head>
	<meta name="viewport" content="width=device-width" />
	<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
	<title>WordPress &#8250; ReadMe</title>
	<link rel="stylesheet" href="wp-admin/css/install.css?ver=20100228" type="text/css" />
</head>
<body>

# 
	[![WordPress](wp-admin/images/wordpress-logo.png)](https://wordpress.org/)

 Version 4.2

Semantic Personal Publishing Platform

# First Things First

Welcome. WordPress is a very special project to me. Every developer and contributor adds something unique to the mix, and together we create something beautiful that I&#8217;m proud to be a part of. Thousands of hours have gone into WordPress, and we&#8217;re dedicated to making it better every day. Thank you for making it part of your world.

&#8212; Matt Mullenweg

# Installation: Famous 5-minute install

1.  Unzip the package in an empty directory and upload everything.
2.  Open <span class="file">[wp-admin/install.php](wp-admin/install.php)</span> in your browser. It will take you through the process to set up a `wp-config.php` file with your database connection details.

        1.  If for some reason this doesn&#8217;t work, don&#8217;t worry. It doesn&#8217;t work on all web hosts. Open up `wp-config-sample.php` with a text editor like WordPad or similar and fill in your database connection details.
    2.  Save the file as `wp-config.php` and upload it.
    3.  Open <span class="file">[wp-admin/install.php](wp-admin/install.php)</span> in your browser.
3.  Once the configuration file is set up, the installer will set up the tables needed for your blog. If there is an error, double check your `wp-config.php` file, and try again. If it fails again, please go to the [support forums](https://wordpress.org/support/ "WordPress support") with as much data as you can gather.
4.  **If you did not enter a password, note the password given to you.** If you did not provide a username, it will be `admin`.
5.  The installer should then send you to the [login page](wp-login.php). Sign in with the username and password you chose during the installation. If a password was generated for you, you can then click on &#8220;Profile&#8221; to change the password.

# Updating

## Using the Automatic Updater

If you are updating from version 2.7 or higher, you can use the automatic updater:

1.  Open <span class="file">[wp-admin/update-core.php](wp-admin/update-core.php)</span> in your browser and follow the instructions.
2.  You wanted more, perhaps? That&#8217;s it!

## Updating Manually

1.  Before you update anything, make sure you have backup copies of any files you may have modified such as `index.php`.
2.  Delete your old WordPress files, saving ones you&#8217;ve modified.
3.  Upload the new files.
4.  Point your browser to <span class="file">[/wp-admin/upgrade.php](wp-admin/upgrade.php).</span>

# Migrating from other systems

WordPress can [import from a number of systems](http://codex.wordpress.org/Importing_Content). First you need to get WordPress installed and working as described above, before using [our import tools](wp-admin/import.php "Import to WordPress").

# System Requirements

*   [PHP](http://php.net/) version **5.2.4** or higher.
*   [MySQL](http://www.mysql.com/) version **5.0** or higher.

## Recommendations

*   [PHP](http://php.net/) version **5.4** or higher.
*   [MySQL](http://www.mysql.com/) version **5.5** or higher.
*   The [mod_rewrite](http://httpd.apache.org/docs/2.2/mod/mod_rewrite.html) Apache module.
*   A link to [wordpress.org](https://wordpress.org/) on your site.

# Online Resources

If you have any questions that aren&#8217;t addressed in this document, please take advantage of WordPress&#8217; numerous online resources:

<dl>
	<dt>[The WordPress Codex](http://codex.wordpress.org/)</dt>
		<dd>The Codex is the encyclopedia of all things WordPress. It is the most comprehensive source of information for WordPress available.</dd>
	<dt>[The WordPress Blog](https://wordpress.org/news/)</dt>
		<dd>This is where you&#8217;ll find the latest updates and news related to WordPress. Recent WordPress news appears in your administrative dashboard by default.</dd>
	<dt>[WordPress Planet](https://planet.wordpress.org/)</dt>
		<dd>The WordPress Planet is a news aggregator that brings together posts from WordPress blogs around the web.</dd>
	<dt>[WordPress Support Forums](https://wordpress.org/support/)</dt>
		<dd>If you&#8217;ve looked everywhere and still can&#8217;t find an answer, the support forums are very active and have a large community ready to help. To help them help you be sure to use a descriptive thread title and describe your question in as much detail as possible.</dd>
	<dt>[WordPress <abbr title="Internet Relay Chat">IRC</abbr> Channel](http://codex.wordpress.org/IRC)</dt>
		<dd>There is an online chat channel that is used for discussion among people who use WordPress and occasionally support topics. The above wiki page should point you in the right direction. ([irc.freenode.net #wordpress](irc://irc.freenode.net/wordpress))</dd>
</dl>

# Final Notes

*   If you have any suggestions, ideas, or comments, or if you (gasp!) found a bug, join us in the [Support Forums](https://wordpress.org/support/).
*   WordPress has a robust plugin <abbr title="application programming interface">API</abbr> that makes extending the code easy. If you are a developer interested in utilizing this, see the [plugin documentation in the Codex](http://codex.wordpress.org/Plugin_API "WordPress plugin API"). You shouldn&#8217;t modify any of the core code.

# Share the Love

WordPress has no multi-million dollar marketing campaign or celebrity sponsors, but we do have something even better&#8212;you. If you enjoy WordPress please consider telling a friend, setting it up for someone less knowledgable than yourself, or writing the author of a media article that overlooks us.

WordPress is the official continuation of [b2/caf&#233;log](http://cafelog.com/), which came from Michel V. The work has been continued by the [WordPress developers](https://wordpress.org/about/). If you would like to support WordPress, please consider [donating](https://wordpress.org/donate/ "Donate to WordPress").

# License

WordPress is free software, and is released under the terms of the <abbr title="GNU General Public License">GPL</abbr> version 2 or (at your option) any later version. See [license.txt](license.txt).

</body>
</html>
Status API Training Shop Blog About
© 2015 GitHub, Inc. Terms Privacy Security Contact
