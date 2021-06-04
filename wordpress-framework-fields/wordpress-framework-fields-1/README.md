# Fields \(59\)

## Code

{% tabs %}
{% tab title="Method 1" %}
{% code title="Function Method" %}
```php
$my_accordion = $my_instance->accordion(array(
  'accordion_1',
  __( 'Accordion' )
);
```
{% endcode %}
{% endtab %}

{% tab title="Method 2" %}
{% code title="Class Method" %}
```php
$my_accordion = $my_instance->accordion(array(
  'accordion_1',
  __( 'Accordion' )
);
```
{% endcode %}
{% endtab %}

{% tab title="Method 3" %}
{% code title="Namespace Method" %}
```php
$my_accordion = $my_instance->accordion(array(
  'accordion_1',
  __( 'Accordion' )
);
```
{% endcode %}
{% endtab %}

{% tab title="Example" %}
```php
$my_accordion = $my_instance->accordion( 'accordion_1', __( 'Accordion' ) );

$my_accordion->text( 'my_text_id', __( 'Text Field' ) );
$my_accordion->textarea( 'my_textarea_id', __( 'Textarea Field' ) );
$my_accordion->checkbox( 'my_checkbox_id', __( 'Checkbox Field' ) );
```
{% endtab %}
{% endtabs %}

## Output

![](../../.gitbook/assets/image%20%289%29.png)

## Tutorial

{% embed url="https://youtu.be/FVqzKAUsM68" %}

## Project Usage



## Notes

There are currently no extra notes for this operation.

