# Field Template

{% hint style="info" %}
Please Do Refer [**Common Arguments**](https://wponion.gitbook.io/docs/fields) For more field options.
{% endhint %}

## Field Related Arguments

| **Option Name**&lt;&gt;//Sample PHP Code |
| --- | --- |


{% tabs %}
{% tab title="First Tab" %}
{% code-tabs %}
{% code-tabs-item title="text.php" %}
```php
array(

);
```
{% endcode-tabs-item %}
{% endcode-tabs %}
{% endtab %}
{% endtabs %}

## Value API

{% hint style="warning" %}
**Note :** Please do use the correct _$instance_ variable.
{% endhint %}

### Get Field Value

```php
$wponion_values = $instance->values();
$field_id_value = $wponion_values->get('{field_id}');
echo $field_id_value->get();
```



