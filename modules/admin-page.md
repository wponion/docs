---
description: WPOnion Module used to create custom pages in wp-admin.
---

# Admin Page

## Arguments

<table>
  <thead>
    <tr>
      <th style="text-align:center">Key</th>
      <th style="text-align:center">Default</th>
      <th style="text-align:left">Description</th>
      <th style="text-align:center">Type</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:center"><b>submenu</b>
      </td>
      <td style="text-align:center">false</td>
      <td style="text-align:left">set parent menu slug to make this menu as sub menu</td>
      <td style="text-align:center"><code>String / false</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:center"><b>menu_title</b>
      </td>
      <td style="text-align:center">false</td>
      <td style="text-align:left">The text to be used for the menu</td>
      <td style="text-align:center"><code>String</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:center"><b>page_title</b>
      </td>
      <td style="text-align:center">false</td>
      <td style="text-align:left">The text to be displayed in the title tags of the page when the menu is
        selected</td>
      <td style="text-align:center"><code>String</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:center"><b>capability</b>
      </td>
      <td style="text-align:center">manage_options</td>
      <td style="text-align:left">The capability required for this menu to be displayed to the user</td>
      <td
      style="text-align:center"><code>String</code>
        </td>
    </tr>
    <tr>
      <td style="text-align:center"><b>menu_slug</b>
      </td>
      <td style="text-align:center">if not provided the it uses <code>page_title / menu_title</code>
      </td>
      <td style="text-align:left">The slug name to refer to this menu by. Should be unique for this menu
        and only include lowercase alphanumeric, dashes, and underscores characters
        to be compatible with <a href="https://developer.wordpress.org/reference/functions/sanitize_key/">sanitize_key()</a>.</td>
      <td
      style="text-align:center"><code>String/Bool</code>
        </td>
    </tr>
    <tr>
      <td style="text-align:center"><b>icon</b>
      </td>
      <td style="text-align:center">false</td>
      <td style="text-align:left">value can be provided only for main menu not for submenu</td>
      <td style="text-align:center"><code>String/false</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:center"><b>position</b>
      </td>
      <td style="text-align:center">false</td>
      <td style="text-align:left">The position in the menu order this one should appear</td>
      <td style="text-align:center"><code>String/false</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:center"><b>on_load</b>
      </td>
      <td style="text-align:center">false</td>
      <td style="text-align:left">
        <p>provided functions / callback will be triggered when page load hook triggers</p>
        <p>uses :<b> load-{page_slug}</b>
        </p>
      </td>
      <td style="text-align:center"><code>callback / array / false</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:center"><b>assets</b>
      </td>
      <td style="text-align:center">false</td>
      <td style="text-align:left">use this to load selected assets only on this page if its loading.</td>
      <td
      style="text-align:center"><code>callback / array / false</code>
        </td>
    </tr>
  </tbody>
</table>\`\`

