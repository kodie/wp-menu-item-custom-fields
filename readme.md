<!-- DO NOT EDIT THIS FILE; it is auto-generated from readme.txt -->
# Menu Item Custom Fields

Easily add custom fields to nav menu items.

**Contributors:** [kucrut](http://profiles.wordpress.org/kucrut)  
**Tags:** [menu](http://wordpress.org/plugins/tags/menu), [nav-menu](http://wordpress.org/plugins/tags/nav-menu), [custom-fields](http://wordpress.org/plugins/tags/custom-fields), [metadata](http://wordpress.org/plugins/tags/metadata)  
**Requires at least:** 3.8  
**Tested up to:** 3.8.1  
**Stable tag:** 0.1.0  
**License:** [GPLv2](http://www.gnu.org/licenses/gpl-2.0.html)  
**Donate Link:** http://kucrut.org/#coffee  

## Description ##

This is a *library* plugin. It doesn't do anything visible on its own. It was written to allow other plugins/themes to add custom fields to menu items *easily*. See **Installation**.

Development of this plugin is done on [GitHub](https://github.com/kucrut/wp-menu-item-custom-fields). **Pull requests welcome**. Please see [issues reported](https://github.com/kucrut/wp-menu-item-custom-fields/issues) there before going to the plugin forum.

## Installation ##

### As regular plugin ###
1. Upload `menu-item-custom-fields` to the `/wp-content/plugins/` directory
1. Activate the plugin through the 'Plugins' menu in WordPress

### As library in your plugin/theme ###
1. Copy `menu-item-custom-fields` to your plugin directory
1. From your plugin file, add this code:
```php
function myplugin_load_menu_item_custom_fields() {
	require_once dirname( __FILE__ ) . '/menu-item-custom-fields/menu-item-custom-fields.php';
}
add_action( 'load-nav-menus.php', 'myplugin_load_menu_item_custom_fields' ) );
```

### Usage ###
Copy (and customize) and include the `menu-item-custom-fields-example.php` file found in the `doc/` directory into your plugin/theme.


## Changelog ##

### 0.1.0 ###
* Initial public release

