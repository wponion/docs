# Settings

## Options {#options}

{% tabs %}
{% tab title="General" %}


| key | value\_type | default\_value | alternative\_values | Description |
| --- | --- | --- | --- | --- | --- | --- |
| extra\_css | Array | `array()` | - | this should contain a array list of registered wp style handle refer [wp\_register\_script](https://developer.wordpress.org/reference/functions/wp_register_script/)​ |
| extra\_js | Array | `array()` | - | this should contain a array of registered wp script handles [wp\_register\_style](https://developer.wordpress.org/reference/functions/wp_register_style/)​ |
| option\_name | String | `_wponion` | any string | this is the database key which is used to store all the settings related data into **wp\_options** table. use any value based on your needs like `_{plugin_slug}_settings` |
| plugin\_id | String | **option\_name** | any string | this key is used to run plugin / current instance related **apply\_filters** / **do\_action** to provide developer easy access to hook with our framework. if this value given empty / false then **option\_name** will be used |
| theme | String | `modern` | any theme slug | Default Available themes \( modern / wp / wp-modern \) |
| template\_path | String | false | Full Path | Provide a full Path where you have your own custom theme / override theme files |
{% endtab %}

{% tab title="Second Tab" %}

{% endtab %}
{% endtabs %}

| key | value\_type | default\_value | alternative\_values | Description |
| --- | --- | --- | --- | --- | --- | --- |
| extra\_css | Array | `array()` | - | this should contain a array list of registered wp style handle refer [wp\_register\_script](https://developer.wordpress.org/reference/functions/wp_register_script/)​ |
| extra\_js | Array | `array()` | - | this should contain a array of registered wp script handles [wp\_register\_style](https://developer.wordpress.org/reference/functions/wp_register_style/)​ |
| option\_name | String | `_wponion` | any string | this is the database key which is used to store all the settings related data into **wp\_options** table. use any value based on your needs like `_{plugin_slug}_settings` |
| plugin\_id | String | **option\_name** | any string | this key is used to run plugin / current instance related **apply\_filters** / **do\_action** to provide developer easy access to hook with our framework. if this value given empty / false then **option\_name** will be used |
| theme | String | `modern` | any theme slug | Default Available themes \( modern / wp / wp-modern \) |
| template\_path | String | false | Full Path | Provide a full Path where you have your own custom theme / override theme files |

## Menu Config {#menu-config}

| key | value\_type | default\_value | alternative\_values | Description |
| --- | --- | --- | --- | --- | --- | --- | --- |
| type | string | theme | Refer Below List of options | ​ |
| title | string | WPOnion | Any String | Title of For the menu |
| slug | string | wponion | Any String | Url slug for the menu |
| capability | string / array | manage\_options | - | Refer [WP Roles\_and\_Capabilities](https://codex.wordpress.org/Roles_and_Capabilities)​ |
| icon | string / url | false | - | custom icon for the menu in wp-admin |
| position | string | false | - | - |
| submenus | bool | false | - | if set to true and the menu type is parent / false then it will add all the first level pages as submenu in wp-admin |

### Menu Type Alternative Values

1. theme
2. management
3. dashboard
4. options
5. plugins
6. theme
7. submenu
8. parent / false

```php
$instance = new WPOnion_Settings(array(        'extra_css'     => array( 'plugin-css-1' ),	'extra_js'      => array( 'plugin-js-1' ),	'option_name'   => '_wpboilerplate_settings',	'template_path' => false,	'menu'          => array(		'type'       => 'parent',		'title'      => 'WP Onion',		'capability' => 'manage_options',		'icon'       => false, # Or Provide A Actual URL of the icon		'position'   => false, #set to false to auto set via wp		'slug'       => 'wponion',		'submenus'   => true,	),	'theme'         => 'wp',	'plugin_id'     => 'boilerplate',));
```



