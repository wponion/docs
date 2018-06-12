# Text

{% hint style="info" %}
Please Do Refer [**Common Arguments**](https://wponion.gitbook.io/docs/fields) For more field options.
{% endhint %}

## Field Related Arguments

| **Option Name** | **Default Value** | **Description** |
| --- | --- | --- | --- |
|  inputmask |  `false` |  |
|  prefix | `false` |  |
|  surfix | `false` |  |

### Example Code & Output

{% tabs %}
{% tab title="Field Array" %}
```php
array(
   'id'    => 'field_id_text',
   'title' => 'Field Title',
   'type'  => 'text',
);
```
{% endtab %}

{% tab title="Masking Array" %}
## Input With Masking

```php
array(
   'id'    => 'field_id_text',
   'title' => 'Field Title',
   'type'  => 'text',
);
```
{% endtab %}
{% endtabs %}

## Value API

{% hint style="warning" %}
**Note :**  _Please Do Replace_ **$instance** _with the exact module's instance variable_
{% endhint %}

### Get Field Value

```php
/**
 * Please Do Replace $instance with the exact module's instance variable
 */
$wponion_values = $instance->values();
$field_id_value = $wponion_values->get('{field_id_text}');
echo $field_id_value->get(); // Returns Fields Value exactly as saved.
```

