# Card

{% hint style="info" %}
Please Do Refer [**Common Arguments**](https://wponion.gitbook.io/docs/fields) For more field options.
{% endhint %}

## Field Related Arguments

| **Option Name** | **Default Value** | **Description** |
| :--- | :--- | :--- |
| **options** | `false` | List of items as array to render. |
| **card\_col** | `col` | Use any bootstrap class. |

### Example Code

{% tabs %}
{% tab title="Field Code" %}
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

{% tab title="Options Array" %}
#### Available Options Array Keys

```php
array(
    'image'           => false,
    'content'         => false, // Use any 1 Body or content.
    'body'            => false,
    'wrap_attributes' => false, // This array will be used for each card wrap div attributes.
    'wrap_class'      => false, // This values will be used for each card wrap div class.
);
```

For more information please [Visit Bootstrap Cards](https://getbootstrap.com/docs/4.1/components/card/).
{% endtab %}
{% endtabs %}

### Output

