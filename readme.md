<!-- DO NOT EDIT THIS FILE; it is auto-generated from readme.txt -->
# Date Range Filter

![Banner](assets/banner-1544x500.png)
Easily filter the admin list of post and custom post type with a date range.

**Contributors:** [jonathanbardo](http://profiles.wordpress.org/jonathanbardo), [stream](http://profiles.wordpress.org/stream)  
**Tags:** [date](http://wordpress.org/plugins/tags/date), [filter](http://wordpress.org/plugins/tags/filter), [admin](http://wordpress.org/plugins/tags/admin), [dashboard](http://wordpress.org/plugins/tags/dashboard)  
**Requires at least:** 3.7  
**Tested up to:** 4.0  
**Stable tag:** trunk (master)  
**License:** [GPLv2 or later](http://www.gnu.org/licenses/gpl-2.0.html)  

## Description ##

**Note: This plugin requires PHP 5.3 or higher to be activated.**

A big shout-out to the [Stream](https://profiles.wordpress.org/stream/) team for developing much of the functionnality of this plugin and letting me reuse it for another purposes. You guys rock!

This plugin was develop to supercharge the current date filter of WordPress admin. It will let you filter posts by a custom date range or by an already defined range.

By default the plugin only filters post creation date. If you would like to filter the post modified date, please use this filter:
```php
function my_date_range_filter_query_column( $column ){
	return 'post_modified';
}
add_filter( 'date_range_filter_query_column', 'my_date_range_filter_query_column', 10, 1 );
```

**Note for developers:**

Is my plugin not giving you enough filters/hooks to play with? Well you are in luck! You can use php class extension to override a part of this plugin. Just create another plugin that extends this one and remove the plugins_loaded action from this plugin and you will be free to do whatever you like! Example [here](https://gist.github.com/jonathanbardo/b837ef296d9883eff2d8).

**Languages Supported:**

 * English

**Improvement? Bugs?**

Please fill out an issue [here](https://github.com/jonathanbardo/WP-Date-Range-Filter/issues).

## Changelog ##

### 0.0.1 ###
Initial release. Props [Stream](https://profiles.wordpress.org/stream/)


