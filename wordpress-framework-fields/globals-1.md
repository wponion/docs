---
description: >-
  These global field options are generally available for all fields. If you find
  any issues using them with any fields please report them to us. Thank you!
---

# Globals

## Basic Values

```php
// ----------------------------------------------------------------------------------------------------
// General Field Options
// ----------------------------------------------------------------------------------------------------

$this_field_demo->title("$this_singular_name Title");
$this_field_demo->horizontal(TRUE); // Set layout to Title above field instead of on left // default FALSE
$this_field_demo->debug(FALSE); // default FALSE
```

## Description Values

```php
// ----------------------------------------------------------------------------------------------------
// Descriptive Field Options
// ----------------------------------------------------------------------------------------------------

$this_field_demo->desc("$this_singular_name descripion"); // Appears below the title
$this_field_demo->desc_field("$this_singular_name descripion"); // Appears below the field

$this_field_demo->before("$this_singular_name descripion"); // Appears above the field
$this_field_demo->after("$this_singular_name descripion"); // Appears below the field

$this_field_demo->wrap_tooltip(
	array(
 		"$this_singular_name Tooltip",
 		'followCursor' => TRUE
	)
);
$this_field_demo->help([
	'icon'    => 'dashicons dashicons-format-status',
	'theme'   => 'light', // default dark
	'size'    => 'large', // Not sure if this changes anythiing in size @Issue
	'content' => __('$this_singular_name Tooltip'),
	'image'   => '', // Full image url
	'onShow'  => 'function(a){ console.log(a);alert("Alert Triggered From PHP");}',
]);
```

## ID, Class & Style Values

```php
// ----------------------------------------------------------------------------------------------------
// Field ID, Classes and Style Options
// ----------------------------------------------------------------------------------------------------

$this_field_demo->wrap_id('custom-field-id'); // Add a custom id to the field's container
$this_field_demo->wrap_class('custom-wrap-class col-xs-12 col-sm-12 col-md-12 col-lg-12 col-xl-12'); // Add a custom class to the field's container or adjust it's flexbox grid values
$this_field_demo->class('custom-field-class'); // Doesn't work with yet or with some fields, may be wrong method name @Issue
$this_field_demo->style('background-color: #000000;'); // Manually enter any inline css styles
$this_field_demo->style(
    array(
        'width' => 'auto',
        'height' => 'auto'
    )
); // Programmatically enter inlin css for the field width and height
```

## Attribute Values

```php
// ----------------------------------------------------------------------------------------------------
// Field Container Attributes and Value Options
// ----------------------------------------------------------------------------------------------------

$this_field_demo->wrap_attribute('attribute-name', 'attribute-value'); // Load a single attribute name and value to the field
$this_field_demo->wrap_attributes(
 array(
  'attribute-name-1' => 'attribute-value-1',
 	'attribute-name-2' => 'attribute-value-2',
 )
); // Load multiple attribute names and values to the field

// ----------------------------------------------------------------------------------------------------
// Field Attributes and Value Options
// ----------------------------------------------------------------------------------------------------

$this_field_demo->attribute('attribute-name', 'attribute-value'); // Load a single attribute name and value to the field
$this_field_demo->attributes(
 array(
  'attribute-name-1' => 'attribute-value-1',
 	'attribute-name-1' => 'attribute-value-2',
 )
); // Load multiple attribute names and values to the field

$this_field_demo->field_default('Defaut_Value_Here'); // Not sure if this works @Issue
```

## Dependency Values

```php
// ----------------------------------------------------------------------------------------------------
// Field Dependency Options
//  $this_container->dependency('field_id_here', 'comparison_method_here', 'value');
// ----------------------------------------------------------------------------------------------------

// DOES EQUAL comparisons

$this_container->dependency('value_here', '=', TRUE);
$this_container->dependency('value_here', '=', '1');
$this_container->dependency('value_here', '=', 'string');

// DOES NOT EQUAL comparisons

$this_container->dependency('value_here', '!=', TRUE);
$this_container->dependency('value_here', '!=', '1');
$this_container->dependency('value_here', '!=', 'string');

// OR comparisons

$this_container->dependency('value_here', 'OR', TRUE);
$this_container->dependency('value_here', 'OR', '1');
$this_container->dependency('value_here', 'OR', 'string');

// ANY comparisons

$this_container->dependency('value_here', 'any', 'value_here_1,value_here_2,value_here_3');
```

## Validation Values

```php
// ----------------------------------------------------------------------------------------------------
// Field Validation Options
//  $this_container->dependency('field_id_here', 'comparison_method_here', 'value');
// ----------------------------------------------------------------------------------------------------

// JS Validation
// @Reference->https://jqueryvalidation.org/

$this_field_demo->js_validate('required'); // Forces field to have an entered value
$this_field_demo->js_validate(['key' => 'required', 'value' => 'required']); // Forces multiple fields to have an entered value
$this_field_demo->js_validate(['minlength' => 10,'maxlength' => 300,]); // Forces field to have a minimum character entered of 10 and max of 300

// PHP Validation

$this_field_demo->validate('wponion_is_required'); // Forces field to have an entered value
$this_field_demo->validate('wponion_is_email'); // Forces field to have a valid email address
$this_field_demo->validate('wponion_is_url'); // Forces field to have a valid url
$this_field_demo->validate(['wponion_is_required' => __('Custom validation message here...')]); // Adds a custom validation message
```

