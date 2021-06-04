# Admin Page

### Menu Arguments

| Key | Options | Description |
| :--- | :--- | :--- |


| **menu\_title** | `false` | The text to be used for the menu |
| :--- | :--- | :--- |


| **page\_title** | `false` | The text to be displayed in the title tags of the page when the menu is selected |
| :--- | :--- | :--- |


| **capability** | `manage_options` | The capability required for this menu to be displayed |
| :--- | :--- | :--- |


<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>menu_slug</b>
      </th>
      <th style="text-align:left">
        <p><code>page_title</code>
        </p>
        <p>/</p>
        <p><code>menu_title</code>
        </p>
      </th>
      <th style="text-align:left">The slug name to refer to this menu by.
        <br />Should be unique for this menu page and only include
        <br />lowercase alphanumeric, dashes, and underscores
        <br />characters to be compatible with <a href="https://developer.wordpress.org/reference/functions/sanitize_key/">sanitize_key()</a>
      </th>
    </tr>
  </thead>
  <tbody></tbody>
</table>

| **position** | `null` | The position in the menu order this one should appear |
| :--- | :--- | :--- |


| **render** | `false` | Callable Function to trigger when page loaded to render output. |
| :--- | :--- | :--- |


| Key | Options | Description |
| :--- | :--- | :--- |


<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>network</b>
      </th>
      <th style="text-align:left"><code>false</code>
      </th>
      <th style="text-align:left">
        <p>Set <code>true</code> if this page can be visible in <b>WP Network Admin</b>
        </p>
        <p>Set <code>only</code> if this page should be visible only in <b>WP Network Admin</b>
        </p>
      </th>
    </tr>
  </thead>
  <tbody></tbody>
</table>

<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>submenu</b>
      </th>
      <th style="text-align:left"><code>false</code>
      </th>
      <th style="text-align:left">
        <p>Pass an <code>array()</code> of menu args to create a <a href="admin-page.md#subemenu-options">submenu</a> under
          current menu</p>
        <p>Pass an <code>string</code> of a menu slug to show current menu under an
          existing menu</p>
        <p>Check <a href="admin-page.md#subemenu-options">submenu</a> section for more
          details</p>
      </th>
    </tr>
  </thead>
  <tbody></tbody>
</table>

<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>on_load</b>
      </th>
      <th style="text-align:left"><code>false</code>
      </th>
      <th style="text-align:left">
        <p>provided functions will be called when current instance page loads.</p>
        <p>uses <b>load-{page_slug} |</b>  <a href="https://codex.wordpress.org/Plugin_API/Action_Reference/load-(page)">Docs</a>
        </p>
      </th>
    </tr>
  </thead>
  <tbody></tbody>
</table>

| **hook\_priority** | `10` | **priority** argument to be passed for `add_action` |
| :--- | :--- | :--- |


| **help\_tab** | `array()` | An array or a callback to render custom help tabs. please check [Help Tabs](help-tabs.md) Module |
| :--- | :--- | :--- |


| **help\_sidebar** | `''` | please check [Help Tab](help-tabs.md)[s](help-tabs.md) Module |
| :--- | :--- | :--- |


| **footer\_text** | `Proudly Powered By WPOnion` | Provide a `string` or a callback function to change text |
| :--- | :--- | :--- |


| **footer\_right\_text** | `WPOnion Version %s` | Provide a `string` or a callback function to change text |
| :--- | :--- | :--- |


### on\_load

{% tabs %}

{% embed url="https://gist.github.com/wponion-framework/cb9b0e46d3ff7323a0cbdc86a41536fc\#file-onload-single-callback-php" caption="" %}

{% embed url="https://gist.github.com/wponion-framework/cb9b0e46d3ff7323a0cbdc86a41536fc\#file-onload-multiple-callback-php" caption="" %}

{% embed url="https://gist.github.com/wponion-framework/cb9b0e46d3ff7323a0cbdc86a41536fc\#file-assets-loading-php" caption="" %}

{% embed url="https://gist.github.com/wponion-framework/f48d58d061c5ab347116012e0b6569e2\#file-single-page-php" caption="" %}

{% embed url="https://gist.github.com/wponion-framework/f48d58d061c5ab347116012e0b6569e2\#file-admin-page-with-submenus-php" caption="" %}

{% embed url="https://gist.github.com/wponion-framework/f48d58d061c5ab347116012e0b6569e2\#file-dashboard-submenu-php" caption="" %}

{% embed url="https://gist.github.com/wponion-framework/f48d58d061c5ab347116012e0b6569e2\#file-multiple-main-menus-php" caption="" %}

{% embed url="https://gist.github.com/wponion-framework/f48d58d061c5ab347116012e0b6569e2\#file-page-with-help-tabs-php" caption="" %}

![](../.gitbook/assets/1541572289-175.gif)

