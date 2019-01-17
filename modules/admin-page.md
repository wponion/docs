# Admin Page

### Menu Arguments

<table>
  <thead>
    <tr>
      <th style="text-align:left">Key</th>
      <th style="text-align:center">Options</th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b>menu_title</b>
      </td>
      <td style="text-align:center"><code>false</code>
      </td>
      <td style="text-align:left">The text to be used for the menu</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>page_title</b>
      </td>
      <td style="text-align:center"><code>false</code>
      </td>
      <td style="text-align:left">The text to be displayed in the title tags of the page
        <br />when the menu is selected</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>capability</b>
      </td>
      <td style="text-align:center"><code>manage_options</code>
      </td>
      <td style="text-align:left">The capability required for this menu to be displayed</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>menu_slug</b>
      </td>
      <td style="text-align:center">
        <p><code>page_title</code>
        </p>
        <p>/</p>
        <p><code>menu_title</code>
        </p>
      </td>
      <td style="text-align:left">The slug name to refer to this menu by.
        <br />Should be unique for this menu page and only include
        <br />lowercase alphanumeric, dashes, and underscores
        <br />characters to be compatible with <a href="https://developer.wordpress.org/reference/functions/sanitize_key/">sanitize_key()</a>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>icon</b>
      </td>
      <td style="text-align:center"><code>none</code>
      </td>
      <td style="text-align:left">The URL to the icon to be used for this menu.
        <br />* <code>base64-encoded</code> SVG using a data URI,
        <br />which will be colored to match the color scheme. <code>data:image/svg+xml;base64</code>
        <br
        />* Name of a Dashicons helper class to use a font icon
        <br />e.g.<code>dashicons-chart-pie</code>
        <br />* Pass <code>none</code> to leave <code>div.wp-menu-image</code>
        <br />empty so an icon can be added via CSS.</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>position</b>
      </td>
      <td style="text-align:center"><code>null</code>
      </td>
      <td style="text-align:left">The position in the menu order this one should appear</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>render</b>
      </td>
      <td style="text-align:center"><code>false</code>
      </td>
      <td style="text-align:left">Callable Function to trigger when page loaded to render output.</td>
    </tr>
  </tbody>
</table>### Additional Arguments

<table>
  <thead>
    <tr>
      <th style="text-align:left">Key</th>
      <th style="text-align:center">Options</th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b>network</b>
      </td>
      <td style="text-align:center"><code>false</code>
      </td>
      <td style="text-align:left">
        <p>Set <code>true</code> if this page can be visible in <b>WP Network Admin</b>
        </p>
        <p>Set <code>only</code> if this page should be visible only in <b>WP Network Admin</b>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>submenu</b>
      </td>
      <td style="text-align:center"><code>false</code>
      </td>
      <td style="text-align:left">
        <p>Pass an <code>array()</code> of menu args to create a <a href="admin-page.md#subemenu-options">submenu</a> under
          current menu</p>
        <p>Pass an <code>string</code> of a menu slug to show current menu under an
          existing menu</p>
        <p>Check <a href="admin-page.md#subemenu-options">submenu</a> section for more
          details</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>on_load</b>
      </td>
      <td style="text-align:center"><code>false</code>
      </td>
      <td style="text-align:left">
        <p>provided functions will be called when current instance page loads.</p>
        <p>uses <b>load-{page_slug} | </b><a href="https://codex.wordpress.org/Plugin_API/Action_Reference/load-(page)">Docs</a>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>assets</b>
      </td>
      <td style="text-align:center"><code>false</code>
      </td>
      <td style="text-align:left">Pass an array or string of Callback Functions / style or script handles
        to trigger when page loaded to <b>enqueue</b> assets</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>hook_priority</b>
      </td>
      <td style="text-align:center"><code>10</code>
      </td>
      <td style="text-align:left"><b>priority</b> argument to be passed for<b> </b><code>add_action</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>help_tab</b>
      </td>
      <td style="text-align:center"><code>array()</code>
      </td>
      <td style="text-align:left">An array or a callback to render custom help tabs.
        <br />please check <a href="help-tabs.md">Help Tabs</a> Module</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>help_sidebar</b>
      </td>
      <td style="text-align:center"><code>&apos;&apos;</code>
      </td>
      <td style="text-align:left">please check <a href="help-tabs.md">Help Tab</a><a href="help-tabs.md">s</a> Module</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>footer_text</b>
      </td>
      <td style="text-align:center"><code>Proudly Powered By WPOnion</code>
      </td>
      <td style="text-align:left">Provide a <code>string</code> or a callback function to change text</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>footer_right_text</b>
      </td>
      <td style="text-align:center"><code>WPOnion Version %s</code>
      </td>
      <td style="text-align:left">Provide a <code>string</code> or a callback function to change text</td>
    </tr>
  </tbody>
</table>## Callbacks

### on\_load

{% tabs %}
{% tab title="Sinle Callback" %}
{% embed url="https://gist.github.com/wponion-framework/cb9b0e46d3ff7323a0cbdc86a41536fc\#file-onload-single-callback-php" %}
{% endtab %}

{% tab title="Multiple Callback" %}
{% embed url="https://gist.github.com/wponion-framework/cb9b0e46d3ff7323a0cbdc86a41536fc\#file-onload-multiple-callback-php" %}
{% endtab %}
{% endtabs %}

### assets

{% embed url="https://gist.github.com/wponion-framework/cb9b0e46d3ff7323a0cbdc86a41536fc\#file-assets-loading-php" %}



## Demo

### Menu & Sub menu's

{% tabs %}
{% tab title="Main Menu" %}
Below code will create a new main admin page.

{% embed url="https://gist.github.com/wponion-framework/f48d58d061c5ab347116012e0b6569e2\#file-single-page-php" %}

![](../.gitbook/assets/1541383988-162.jpg)
{% endtab %}

{% tab title="Main Menu & Sub menu" %}
{% embed url="https://gist.github.com/wponion-framework/f48d58d061c5ab347116012e0b6569e2\#file-admin-page-with-submenus-php" %}

![](../.gitbook/assets/1541468326-122.gif)
{% endtab %}
{% endtabs %}

### WP Sub menus

{% tabs %}
{% tab title="Dashboard" %}
{% embed url="https://gist.github.com/wponion-framework/f48d58d061c5ab347116012e0b6569e2\#file-dashboard-submenu-php" %}

![](../.gitbook/assets/1541384688-137.jpg)
{% endtab %}
{% endtabs %}

### Multiple Main Menus

{% embed url="https://gist.github.com/wponion-framework/f48d58d061c5ab347116012e0b6569e2\#file-multiple-main-menus-php" %}

![](../.gitbook/assets/1541466937-141.jpg)

### Page With Help Tabs

{% embed url="https://gist.github.com/wponion-framework/f48d58d061c5ab347116012e0b6569e2\#file-page-with-help-tabs-php" %}

![](../.gitbook/assets/1541572289-175.gif)



