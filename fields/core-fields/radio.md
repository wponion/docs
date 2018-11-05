# Radio

{% hint style="info" %}
Please Do Refer [**Common Arguments**](https://wponion.gitbook.io/docs/fields) For more field options.
{% endhint %}

## Field Related Arguments <a id="field-related-arguments"></a>

| **Option Name** | **Default Value** | **Description** |
| :--- | :--- | :--- |
|  label | `​false` | ​ |
|  options | `array()` |  |

### Example Code & Output <a id="example-code-and-output"></a>

```php
array(
    'id'    => 'field_id_radio',
    'title' => 'Field Title',
    'type'  => 'radio',
);
```

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
$field_id_value = $wponion_values->get('{field_id_radio}');
echo $field_id_value->get(); // Returns Fields Value exactly as saved.
```

