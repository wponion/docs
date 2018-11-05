# Textarea

{% hint style="info" %}
Please Do Refer [**Common Arguments**](https://wponion.gitbook.io/docs/fields) For more field options.
{% endhint %}

## Field Related Arguments

| **Option Name** | **Default Value** | **Description** |
| :--- | :--- | :--- |
|  rows | `5` |  |
|  col | `5` |  |
|  inputmask |  `false` |  |
|  prefix |  `false` |  |
|  surfix |  `false` |  |

### Example Code & Output

{% tabs %}
{% tab title="Field Array" %}
```php
array(
    'id'    => 'field_id_textarea',
    'title' => 'Field Title',
    'type'  => 'textarea',
);
```
{% endtab %}

{% tab title="Masking Array" %}
## Input With Masking <a id="input-with-masking"></a>
{% endtab %}
{% endtabs %}

## Value API <a id="value-api"></a>

{% hint style="warning" %}
**Note :** _Please Do Replace_ **$instance** _with the exact module's instance variable_
{% endhint %}

### Get Field Value <a id="get-field-value"></a>

```php
/**
 * Please Do Replace $instance with the exact module's instance variable
 */
$wponion_values = $instance->values();
$field_id_value = $wponion_values->get('{field_id_textarea}');
echo $field_id_value->get(); // Returns Fields Value exactly as saved.
```

