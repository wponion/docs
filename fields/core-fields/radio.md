# Radio

{% hint style="info" %}
Please Do Refer [**Common Arguments**](https://wponion.gitbook.io/docs/fields) For more field options.
{% endhint %}

## Field Related Arguments {#field-related-arguments}

| **Option Name** | **Default Value** | **Description** |
| --- | --- | --- |
|  label | `​false` | ​ |
|  options | `array()` |  |

### Example Code & Output {#example-code-and-output}

```php
array(
    'id'    => 'field_id_radio',
    'title' => 'Field Title',
    'type'  => 'radio',
);
```

## Value API {#value-api}

{% hint style="warning" %}
**Note :** _Please Do Replace_ **$instance** _with the exact module's instance variable_
{% endhint %}

### Get Field Value {#get-field-value}

```php
/**
 * Please Do Replace $instance with the exact module's instance variable
 */
$wponion_values = $instance->values();
$field_id_value = $wponion_values->get('{field_id_radio}');
echo $field_id_value->get(); // Returns Fields Value exactly as saved.
```

