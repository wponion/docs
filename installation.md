# Installation

## Include In Theme

* Extract download zip on your-theme-name/wponion folder under your theme directory 
* Add framework include code on your theme your-theme-name/functions.php file
* Yay! Right now you are ready to configure framework, metaboxes, taxonomies, wp customize, shortcode
* Take a look for config files from your-theme-name/wpsf-framework/config folder
* Read for about configuration

> ### Folder Structure

```php
├── wp-content
|   ├── themes
|   |   ├── themename
|   |   ├── functions.php
|   |   ├── ...
|   |   ├── ...
```

> This is not meant replace your main functions.php, only put this code below your codes

```php
/**
 * WPSFramework
 * A Lightweight and easy-to-use WordPress Options Framework
 */
require_once get_template_directory_uri() .'/wpsf-framework/wpsf-framework.php';
​
// -( or )-
// require_once get_template_directory_uri() .'/subfolder/wpsf-framework/wpsf-framework.php';
```

## Include In plugin

* Extract download zip on your-plugin/wponion folder under your theme directory
* Add framework include code on your theme your-plugin/functions.php file
* Yay! Right now you are ready to configure framework, metaboxes, taxonomies, wp customize, shortcode
* Take a look for config files from your-plugin/wponion/config folder
* Read for about configuration

> ### Folder Structure

```text
├── wp-content
|   ├── plugins
|   |   ├── your-plugin
|   |   |   ├── your-plugin.php
|   |   |   ├── functions.php
```

> Add the below code in plugin's main file your-plugin.php

```php
/**
 * wponion
 * A Lightweight and easy-to-use WordPress Options Framework
 */
require_once plugin_dir_path(__FILE__) .'/wponion/wponion-framework.php';
```

## Usage as Standalone Plugin

* Way1 Extract download zip on wp-content/plugins/wponion folder under your plugin directory
* Way  Upload zip file from wordpess plugins panel -&gt; add new -&gt; upload plugin
* Active wponion plugin from wordpress plugins panel
* Yay! Right now you are ready to configure framework, metaboxes, taxonomies, wp customize, shortcode
* Take a look for config files from wp-content/plugins/wponion/config folder also you can manage config files from theme directory. see overriding files method.
* Read for about configuration

```text
├── wp-content
|   ├── plugins
|   |   ├── akismet
|   |   ├── wponion
|   |   ├── ...
|   |   ├── ...
```

