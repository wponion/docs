---
description: >-
  This Module can be used to add custom columns to tables that uses
  WP_List_Table
---

# Admin Columns

## Arguments

<table>
  <thead>
    <tr>
      <th style="text-align:left">Key</th>
      <th style="text-align:left">Default</th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b>post_type</b>
      </td>
      <td style="text-align:left"><code>false</code>
      </td>
      <td style="text-align:left">
        <p><code>array()</code> or <code>string</code> of a post type slug.</p>
        <p>if provided & none of them matches current
          <br />post type then column will not be rendered</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>name</b>
      </td>
      <td style="text-align:left"><code>title</code>/ <code>false</code>
      </td>
      <td style="text-align:left">Column Slug. if not provided then
        <br />it uses <code>title</code> attribute value</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>title</b>
      </td>
      <td style="text-align:left"><code>false</code>
      </td>
      <td style="text-align:left">Column Title</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>render</b>
      </td>
      <td style="text-align:left"><code>false</code>
      </td>
      <td style="text-align:left">String / Array of callback to render output.</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>reorder</b>
      </td>
      <td style="text-align:left"><code>false</code>
      </td>
      <td style="text-align:left">provide a column slug to show after it or
        <br />a callable function to do custom reordering</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
  </tbody>
</table>## Demo

### Custom Column In Default Post - Post Type

![](https://vsp.ams3.cdn.digitaloceanspaces.com/sshots/i/2019/Jan/17/1547705103-165.jpg)

{% embed url="https://gist.github.com/wponion-framework/c9c91c3c888346c3b69bc92498eca260\#file-admin-columns-php" %}

### Column Reorder Options

![](https://vsp.ams3.cdn.digitaloceanspaces.com/sshots/i/2019/Jan/17/1547705134-169.jpg)

{% embed url="https://gist.github.com/wponion-framework/c9c91c3c888346c3b69bc92498eca260\#file-admin-columns-reorder-php" %}

### Multiple Columns @ Once

![](../../.gitbook/assets/image.png)

{% embed url="https://gist.github.com/wponion-framework/c9c91c3c888346c3b69bc92498eca260\#file-admin-columns-multiple-php" %}



