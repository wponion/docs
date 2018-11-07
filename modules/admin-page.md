---
description: WPOnion Module used to create custom pages in wp-admin.
---

# Admin Page

## Module Arguments

<table>
  <thead>
    <tr>
      <th style="text-align:left">Key</th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b>submenu</b>
      </td>
      <td style="text-align:left">set parent menu slug to make this menu as sub menu</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>menu_title</b>
      </td>
      <td style="text-align:left">The text to be used for the menu</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>page_title</b>
      </td>
      <td style="text-align:left">The text to be displayed in the title tags of the page when the menu is
        selected</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>capability</b>
      </td>
      <td style="text-align:left">
        <p>The capability required for this menu to be displayed to the user</p>
        <p><code>Default : manage_option</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>menu_slug</b>
      </td>
      <td style="text-align:left">
        <p>The slug name to refer to this menu by. Should be unique for this menu
          and only include lowercase alphanumeric, dashes, and underscores characters
          to be compatible with <a href="https://developer.wordpress.org/reference/functions/sanitize_key/">sanitize_key()</a>.</p>
        <p></p>
        <p><code>if no value provided then it uses page_title / menu_title</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>icon</b>
      </td>
      <td style="text-align:left">value can be provided only for main menu not for submenu</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>position</b>
      </td>
      <td style="text-align:left">The position in the menu order this one should appear</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>on_load</b>
      </td>
      <td style="text-align:left">
        <p>provided functions / callback will be triggered when page load hook triggers</p>
        <p>uses :<b> load-{page_slug}</b>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>assets</b>
      </td>
      <td style="text-align:left">use this to load selected assets only on this page if its loading.</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>render</b>
      </td>
      <td style="text-align:left">provide a custom function to call when page needs to render</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>help_tab</b>
      </td>
      <td style="text-align:left">An array or a callback to render custom help tabs. please check <a href="help-tabs.md">Help Tabs</a> Module</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>help_sidebar</b>
      </td>
      <td style="text-align:left">please check <a href="help-tabs.md">Help Tab</a><a href="help-tabs.md">s</a> Module</td>
    </tr>
  </tbody>
</table>### Callback Types

**`on_load`** , **`assets`** , **`callback`** / **`render`**  

all of the above mentioned arguments can handle any type of callback like \( hook  or function \)  
for more information please check the demo

## Demo

### Menu & Sub menu's

{% tabs %}
{% tab title="Main Menu" %}
Below code will create a new main admin page.

{% code-tabs %}
{% code-tabs-item title="wponion-admin-page.php" %}
```php
function wponion_render_demo_page() {
	echo 'This is a demo page';
}
wponion_admin_page( array(
	'menu_title' => __( 'WPOnion Demo' ),
	'page_title' => __( 'WPOnion Admin Page Module' ),
	'menu_slug'  => 'wponion-demo',
	'render'     => 'wponion_render_demo_page',
) );
```
{% endcode-tabs-item %}
{% endcode-tabs %}

![](../.gitbook/assets/1541383988-162.jpg)
{% endtab %}

{% tab title="Main Menu & Sub menu" %}
{% code-tabs %}
{% code-tabs-item title="wponion-main-menu-sub-menu.php" %}
```php
function wponion_render_demo_page() {
	echo 'This is a demo page';
}

$parent = wponion_admin_page( array(
	'submenu'    => array(
		'menu_title' => __( 'Submenu 1' ),
		'page_title' => __( 'Submenu 1' ),
		'menu_slug'  => 'submenu-1',
		'render'     => 'wponion_render_demo_page',
	),
	'menu_title' => __( 'WPOnion Demo' ),
	'page_title' => __( 'WPOnion Admin Page Module' ),
	'menu_slug'  => 'wponion-demo',
	'render'     => 'wponion_render_demo_page',
) );

wponion_admin_page( array(
	'submenu'    => $parent,
	'menu_title' => __( 'Subemnu 2' ),
	'page_title' => __( 'Submenu 2' ),
	'menu_slug'  => 'submenu-2',
	'render'     => 'wponion_render_demo_page',
) );

wponion_admin_page( array(
	'submenu'    => array(
		array(
			'menu_title' => __( 'WPO Submenu 1' ),
			'page_title' => __( 'WPO Submenu 1' ),
			'menu_slug'  => 'wpo-submenu-1',
			'render'     => 'wponion_render_demo_page',
		),
		array(
			'menu_title' => __( 'WPO Submenu 2' ),
			'page_title' => __( 'WPO Submenu 2' ),
			'menu_slug'  => 'wpo-submenu-1',
			'render'     => 'wponion_render_demo_page',
		),
	),
	'menu_title' => __( 'WPO Demo 2 ' ),
	'page_title' => __( 'WPOnion Admin Page Module - 2' ),
	'menu_slug'  => 'wponion-demo-2',
	'render'     => 'wponion_render_demo_page',
) );
```
{% endcode-tabs-item %}
{% endcode-tabs %}

![](../.gitbook/assets/1541468326-122.gif)
{% endtab %}
{% endtabs %}

### WP Sub menus

{% tabs %}
{% tab title="Dashboard" %}
{% code-tabs %}
{% code-tabs-item title="wponion-dashboard-menu.php" %}
```php
function wponion_render_demo_page() {
	echo 'This is a demo page';
}

wponion_admin_page( array(
    'submenu'    => 'dashboard',
    'menu_title' => __( 'WPOnion Demo' ),
    'page_title' => __( 'WPOnion Admin Page Module' ),
    'menu_slug'  => 'wponion-demo',
    'render'     => 'wponion_render_demo_page',
) );
```
{% endcode-tabs-item %}
{% endcode-tabs %}

![](../.gitbook/assets/1541384688-137.jpg)
{% endtab %}

{% tab title="Second Tab" %}

{% endtab %}
{% endtabs %}

### Multiple Main Menus

{% code-tabs %}
{% code-tabs-item title="wponion-multiple-main-menus.php" %}
```php
function wponion_render_demo_page() {
	echo 'This is a demo page';
}

function wponion_render_demo_page2() {
	echo 'This is a demo page';
}

wponion_admin_page( array(
	array(
		'menu_title' => __( 'WPOnion Demo 1' ),
		'page_title' => __( 'WPOnion Admin Page Module 1' ),
		'menu_slug'  => 'wponion-demo-1',
		'render'     => 'wponion_render_demo_page',
	),
	array(
		'menu_title' => __( 'WPOnion Demo 2' ),
		'page_title' => __( 'WPOnion Admin Page Module 2' ),
		'menu_slug'  => 'wponion-demo-2',
		'render'     => 'wponion_render_demo_page2',
	),
) );
```
{% endcode-tabs-item %}
{% endcode-tabs %}

![](../.gitbook/assets/1541466937-141.jpg)

### Page With Help Tabs

```php
wponion_admin_page( array(
   'submenu'      => 'dashboard',
   'menu_title'   => __( 'WPOnion Demo' ),
   'page_title'   => __( 'WPOnion Admin Page Module' ),
   'menu_slug'    => 'wponion-demo',
   'help_tab'     => array(
      'Tab 1' => array(
         'content' => 'Tab 1 content here ...',
      ),
      'Tab 2' => array(
         'content' => 'Tab 1 content here ...',
      ),
   ),
   'help_sidebar' => 'Some Content',
   'render'       => 'wponion_render_demo_page',
) );
```

![](../.gitbook/assets/1541572289-175.gif)

## On Load Hook

### Single Callback

{% code-tabs %}
{% code-tabs-item title="wponion-admin-page-callback.php" %}
```php
wponion_admin_page( array(
	'submenu'    => 'dashboard',
	'menu_title' => __( 'WPOnion Demo' ),
	'page_title' => __( 'WPOnion Admin Page Module' ),
	'menu_slug'  => 'wponion-demo',
	'on_load'    => 'wponion_page_on_load',
) );

function wponion_page_on_load() {
	// This function is called when WPOnion Demo page is loaded.
}
```
{% endcode-tabs-item %}
{% endcode-tabs %}

### Multiple Callback

{% code-tabs %}
{% code-tabs-item title="wponion-callback.php" %}
```php
class WPOnion_Demo_Page {
	public static function on_load_callback() {
		// This function is called when WPOnion Demo page is loaded.
	}
}

add_action( 'on_load_callback_hook', 'on_load_callback_function' );

function on_load_callback_function() {
	// This function is called when WPOnion Demo page is loaded.
}

wponion_admin_page( array(
	'submenu'    => 'dashboard',
	'menu_title' => __( 'WPOnion Demo' ),
	'page_title' => __( 'WPOnion Admin Page Module' ),
	'menu_slug'  => 'wponion-demo',
	'on_load'    => array(
		'on_load_callback_function',
		'on_load_callback_hook',
		array( 'WPOnion_Demo_Page', 'on_load_callback' ),
		function () {
			// This function is called when WPOnion Demo page is loaded.
		},
	),
) );

```
{% endcode-tabs-item %}
{% endcode-tabs %}

