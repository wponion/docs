# Include In Theme

* Extract download zip on `your-theme-name/wponion` folder under your theme directory 
* Add framework include code on your theme `your-theme-name/functions.php` file
* Yay! Right now you are ready to configure framework, metaboxes, taxonomies, wp customize, shortcode
* Take a look for config files from `your-theme-name/wponion` folder
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

> This is not meant replace your main **`functions.php`**, only put this code below your codes

```php
/**
 * WPSFramework
 * A Lightweight and easy-to-use WordPress Options Framework
 */
require_once get_template_directory_uri() .'/wponion/wponion.php';
​
// -( or )-
// require_once get_template_directory_uri() .'/subfolder/wponion/wponion.php';
```

