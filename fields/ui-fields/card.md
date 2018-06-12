# Card

{% hint style="info" %}
Please Do Refer [**Common Arguments**](https://wponion.gitbook.io/docs/fields) For more field options.
{% endhint %}

## Field Related Arguments

| **Option Name** | **Default Value** | **Description** |
| --- | --- | --- |
| **options** | `false` | List of items as array to render. |
| **card\_col** | `col` | Use any bootstrap class. |

### Example Code

{% tabs %}
{% tab title="Second Tab" %}
```php
array(
    'type'     => 'card',
    'options'  => array(
        array(
            'image'   => 'http://via.placeholder.com/200x200',
            'content' => 'Here your content.',
        ),

        array(
            'image'   => 'http://via.placeholder.com/200x200',
            'content' => 'Here your content.',
        ),

        array(
            'image'   => 'http://via.placeholder.com/200x200',
            'content' => 'Here your content.',
        ),

        array(
            'image'   => 'http://via.placeholder.com/200x200',
            'content' => 'Here your content.',
        ),

    ), // Refer Options Tab Above.
    'card_col' => 'col',
);
```
{% endtab %}
{% endtabs %}

### Output



