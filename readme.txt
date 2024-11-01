=== WP Dropdown Posts ===
Author: takien
Contributors: takien
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=BL7ERUY46HPL8&lc=ID&item_name=WP%20Dropdown%20Posts%20Plugin&currency_code=USD&bn=PP%2dDonationsBF%3abtn_donate_SM%2egif%3aNonHosted
Tags: post, dropdown, jump, menu
Tested up to: 0.2
Stable tag: 0.2

This plugin will show post list as dropdown

== Description ==

This plugin will show post list as dropdown just like wp_dropdown_pages, most parameter wp_dropdown_pages are accepted too.

== Screenshots ==

1. Wp Dropdown Posts
2. Long titles will not break your dropdown (version 0.2);

== Installation ==

1. Upload the `wp-dropdown-posts.php` file to the `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress
3. Paste the following code to your theme file, e.g in your sidebar.php

`<?php wp_dropdown_posts('sort_column=post_date&sort_order=DESC&number=10&cut_word=1&cut_limit=20&cut_replacement=...'); ?>`

That will show latest 10 posts in dropdown. Title that has more than 20 characters will be truncated.

= Parameter = 
* sort_order
* sort_column
* exclude
* include
* meta_key
* meta_value
* authors
* number
* offset
* name
* show_option_none
* show_option_no_change
* option_none_value

Description about above parameters can be found here http://codex.wordpress.org/Template_Tags/wp_dropdown_pages#Other_Parameters

* jump_to, if is set to 0, the dropdown will not clickable, default 1
* cut_word, set to 1 to cut long titles, default 0
* cut_limit, number of first characters will be shown, default 30
* cut_replacement, the replacement of truncated characters, default ... 

== Changelog ==
= 0.2 =
* Add feature to show only first x title characters, so the dropdown will not spreaded.
* New parameter: cut_word, cut_limit, cut_replacement

= 0.1 =
* First release