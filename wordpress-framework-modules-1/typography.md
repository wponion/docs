# Typography

## Code

{% tabs %}
{% tab title="Function" %}
```php
wponion_admin_bar( 
    array($title, $href, $id, $meta, $parent, $group, $submenus)
);
```
{% endtab %}

{% tab title="Example" %}
```php
wponion_admin_bar(
  array(
    array(
      'title' => 'My_Menu_Title',
      'href' => 'https://mycustomlink.com',
      'id' => 'my-custom-html-id',
      'parent' => array(
        'children' => array(),
      ),
      'group' => array(),
      'meta' => array(
        'title' => 'my-custom-meta-title',
        'class' => 'my-custom-meta-class',
        'id' => 'my-custom-meta-id',
        'target' => 'self',
        'onclick' => NULL,
        'rel' => NULL,
        'tab' => NULL,
        'lang' => NULL,
        'dir' => NULL,
      ),
      'submenus' => array(
        array(
          'title' => 'My_Menu_Title',
          'href' => 'https://mycustomlink.com',
          'id' => 'my-custom-html-id',
          'meta' => array(
            'title' => 'my-custom-meta-title',
            'class' => 'my-custom-meta-class',
            'id' => 'my-custom-meta-id',
            'target' => 'self',
            'onclick' => NULL,
            'rel' => NULL,
            'tab' => NULL,
            'lang' => NULL,
            'dir' => NULL,
          ),
        ),
      ),
    ),
  ),
);
```
{% endtab %}
{% endtabs %}

## Output

![](../.gitbook/assets/image%20%289%29.png)

## Tutorial

{% embed url="https://youtu.be/FVqzKAUsM68" %}

## Project Usage



## Notes

There are currently no extra notes for this operation.

