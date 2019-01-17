---
description: Module to hook with WordPress Bulk Edit.
---

# Bulk Edit

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
      <td style="text-align:left"><b>option_name</b>
      </td>
      <td style="text-align:left"><code>null</code>
      </td>
      <td style="text-align:left"><b>Meta Key </b><em><code>[ WP Meta Table ]</code></em><b><br /></b>used
        to either retrieve / update the values in DB</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>post_type</b>
      </td>
      <td style="text-align:left"><code>array()</code>
      </td>
      <td style="text-align:left">
        <p>List of Post Type Support.</p>
        <p>Post Type that are passed will be hooked and render bulk edit</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>column</b>
      </td>
      <td style="text-align:left"><code>null</code>
      </td>
      <td style="text-align:left">Provide a valid Column Slug to hook with and enable Bulk Edit</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>values</b>
      </td>
      <td style="text-align:left"><code>null</code>
      </td>
      <td style="text-align:left">Custom Argument to pass DB values. it can either be an array of values
        or a function callback which returns the values.</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>save</b>
      </td>
      <td style="text-align:left"><code>false</code>
      </td>
      <td style="text-align:left">
        <p>Custom save handler. to handle saving data in db.</p>
        <p>should be a callable function.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>wrap_class</b>
      </td>
      <td style="text-align:left"><code>&apos;&apos;</code>
      </td>
      <td style="text-align:left">
        <p>Custom Wrap Class which will appended to HTML Output.</p>
        <p>This can be used to write custom styling</p>
      </td>
    </tr>
  </tbody>
</table>## Demo

![](https://vsp.ams3.cdn.digitaloceanspaces.com/sshots/i/2019/Jan/17/1547729219-122.jpg)

{% embed url="https://gist.github.com/wponion-framework/d2c379a3fb93ab42b145a031d3c1bd26" %}



