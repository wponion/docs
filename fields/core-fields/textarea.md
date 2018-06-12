# Textarea

{% hint style="info" %}
Please Do Refer [**Common Arguments**](https://wponion.gitbook.io/docs/fields) For more field options.
{% endhint %}

## Field Related Arguments

| **Option Name** | **Default Value** | **Description** |
| --- | --- |
|  |  |  |

## Example Code & Output

{% tabs %}
{% tab title="First Tab" %}
## Input With Masking {#input-with-masking}

```php
array(
    'id'    => 'field_id',
    'title' => 'Field Title',
    'type'  => 'text',
);
```
{% endtab %}

{% tab title="Second Tab" %}

{% endtab %}
{% endtabs %}

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
$field_id_value = $wponion_values->get('{field_id}');
echo $field_id_value->get(); // Returns Fields Value exactly as saved.
```

