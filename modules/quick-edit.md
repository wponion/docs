---
description: Module to hook with WordPress Bulk Edit.
---

# Quick Edit

## Arguments <a id="arguments"></a>

| Key | Default | Description |
| :--- | :--- | :--- |


| **option\_name** | `null` | **Meta Key** _`[ WP Meta Table ]`_ used to either retrieve / update the values in DB |
| :--- | :--- | :--- |


<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>post_type</b>
      </th>
      <th style="text-align:left"><code>array()</code>
      </th>
      <th style="text-align:left">
        <p>List of Post Type Support.</p>
        <p>Post Type that are passed will be hooked and render Quick edit</p>
      </th>
    </tr>
  </thead>
  <tbody></tbody>
</table>

| **column** | `null` | Provide a valid Column Slug to hook with and enable Quick Edit |
| :--- | :--- | :--- |


| **values** | `null` | Custom Argument to pass DB values. it can either be an array of values or a function callback which returns the values. |
| :--- | :--- | :--- |


<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>save</b>
      </th>
      <th style="text-align:left"><code>false</code>
      </th>
      <th style="text-align:left">
        <p>Custom save handler. to handle saving data in db.</p>
        <p>should be a callable function.</p>
      </th>
    </tr>
  </thead>
  <tbody></tbody>
</table>

<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>wrap_class</b>
      </th>
      <th style="text-align:left"><code>&apos;&apos;</code>
      </th>
      <th style="text-align:left">
        <p>Custom Wrap Class which will appended to HTML Output.</p>
        <p>This can be used to write custom styling</p>
      </th>
    </tr>
  </thead>
  <tbody></tbody>
</table>

![](https://vsp.ams3.cdn.digitaloceanspaces.com/sshots/i/2019/Jan/17/1547729438-1100.jpg)

{% embed url="https://gist.github.com/wponion-framework/e6aac3c3b08d1792ded08b0c5bcf7e81" caption="" %}

