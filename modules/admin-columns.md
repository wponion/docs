# Admin Columns

## Arguments

| Key | Default | Description |
| :--- | :--- | :--- |


<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>post_type</b>
      </th>
      <th style="text-align:left"><code>false</code>
      </th>
      <th style="text-align:left">
        <p><code>array()</code> or <code>string</code> of a post type slug.</p>
        <p>if provided &amp; none of them matches current
          <br />post type then column will not be rendered</p>
      </th>
    </tr>
  </thead>
  <tbody></tbody>
</table>

| **name** | `title`/ `false` | Column Slug. if not provided then it uses `title` attribute value |
| :--- | :--- | :--- |


| **title** | `false` | Column Title |
| :--- | :--- | :--- |


| **render** | `false` | String / Array of callback to render output. |
| :--- | :--- | :--- |


| **reorder** | `false` | provide a column slug to show after it or a callable function to do custom reordering |
| :--- | :--- | :--- |


|  |  |  |
| :--- | :--- | :--- |


### Custom Column In Default Post - Post Type

![](https://vsp.ams3.cdn.digitaloceanspaces.com/sshots/i/2019/Jan/17/1547705103-165.jpg)

{% embed url="https://gist.github.com/wponion-framework/c9c91c3c888346c3b69bc92498eca260\#file-admin-columns-php" caption="" %}

{% embed url="https://gist.github.com/wponion-framework/c9c91c3c888346c3b69bc92498eca260\#file-admin-columns-reorder-php" caption="" %}

{% embed url="https://gist.github.com/wponion-framework/c9c91c3c888346c3b69bc92498eca260\#file-admin-columns-multiple-php" caption="" %}

