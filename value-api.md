---
description: >-
  Value API is a builtin class which helps you to get the stored value easily.
  just by calling few functions. instead of checking into an array.
---

# Value API

## Supported Modules

* Settings
* Taxonomy
* Metabox
* WC Metabox
* User Profile
* Customizer
* Widgets
* Gutenberg
* Visual Composer

### _Settings / Customizer_ Module's Value

Here we will be using **`$instance`** variable in which a module's class instance will be stored.  
and with the below code we will be able to get the modules stored data.

```php
/**
 * $instance variable should be an instance of any of the below
 * \WPOnion\Modules\Settings
 * \WPOnion\Modules\Customizer
 */
$values = $instance->values();
```

## Built In Functions

### get\(\)

Get function can be used either to get a field's value or a sub fields instance. below is an example

{% tabs %}
{% tab title="First Tab" %}
```php
/**
 * Here we are using $values which is a base instance of value 
 * which had stored all the fields of the modules and its value.
 * Here we are using get along with a field ID to get its field value api instance.
 */
$subfield1 =$values->get('first_fieldset');
print_r($subfield1);

$subfield2 = $subfield1->get('second_fieldset');
print_r($subfield2);

$subfield3 = $subfield2->get('second_fieldset_text');
echo $subfield3;
```
{% endtab %}

{% tab title="Second Tab" %}

{% endtab %}
{% endtabs %}

### raw\(\)

### html\(\)

### active\(\)

