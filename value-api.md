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

{% hint style="info" %}
**NOTE** for each and every field a new **VALUE API** instance will be created and stored in the base  
**VALUE API** instance variable \( `$values` \)
{% endhint %}

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


/**
 * Here we are using Subfield1 variable to get a subfield which is nested into the first_fieldset
 */
$subfield2 = $subfield1->get('second_fieldset');
print_r($subfield2);


/**
 * Here we are using $subfield2 to get a text field value from the 2nd nested level
 * You can either echo directly or use any of the functions which are given blow
 * raw() | html() 
 * please do refer the field's doc to know more about field specific functions
 */
$subfield3 = $subfield2->get('second_fieldset_text');
echo $subfield3;

/**
 * You can also use below option to get 2nd level text field value
 * here it will return the value of $subfeild3
 */
 echo $subfield1->get('second_fieldset.second_fieldset_text');
```
{% endtab %}

{% tab title="Second Tab" %}

{% endtab %}
{% endtabs %}

### raw\(\)

### html\(\)

### active\(\)

