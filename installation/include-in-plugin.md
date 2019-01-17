# Include In plugin

* Extract download zip on `your-plugin/wponion` folder under your theme directory
* Add framework include code on your theme `your-plugin/functions.php` file
* Yay! Right now you are ready to configure framework, metaboxes, taxonomies, wp customize, shortcode
* Take a look for config files from `your-plugin/wponion/config` folder
* Read for about configuration

> ### Folder Structure

```text
├── wp-content
|   ├── plugins
|   |   ├── your-plugin
|   |   |   ├── your-plugin.php
|   |   |   ├── functions.php
```

> Add the below code in plugin's main file **`your-plugin.php`**

```php
/**
 * wponion
 * A Lightweight and easy-to-use WordPress Options Framework
 */
require_once plugin_dir_path(__FILE__) .'/wponion/wponion-framework.php';
```

