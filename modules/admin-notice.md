# Admin Notice

## Arguments

| Key | Default | Description |
| :--- | :--- | :--- |
| **content** | `null` | Notice Content |
| **title** | `null` | Notice Title |
| **type** | `success` | `succcess` / `info` / `warning` / `error` / `updated` / `update-nag` |
| **times** | `1` | No of times to show this notice |
| **screens** | `array()` | array of screen ids to render notice only in those screens |
| **users** | `array()` | array of user ids to render notice only for those users |
| **large** | `false` | Render notice in large layout |
| **alt** | `false` | if set to true then it renders notice in alternate site for the given notice type |
| **inline** | `false` | if set to true then WordPress will not move this notice to top of the page |
| **dismissible** | `true` | if set to true then it appends a clone button to notice |

{% hint style="info" %}
**Note :**  For Each Notice Type WPOnion Builtin Function To Render It Quickly
{% endhint %}

* Success : `wponion_success_admin_notice`
* Info : `wponion_info_admin_notice`
* Warning : `wponion_warning_admin_notice`
* Error : `wponion_error_admin_notice`
* Upgrade-Nag : `wponion_upgrade_admin_notice`

## Demo

### Basic Config

![](https://vsp.ams3.cdn.digitaloceanspaces.com/sshots/i/2019/Jan/17/1547710698-169.jpg)

{% embed url="https://gist.github.com/wponion-framework/44c457ba6c9cd64a5861a4eb7149e3b1\#file-basic-config-php" %}

### Success

![](https://vsp.ams3.cdn.digitaloceanspaces.com/sshots/i/2019/Jan/17/1547709941-18.jpg)

{% embed url="https://gist.github.com/wponion-framework/44c457ba6c9cd64a5861a4eb7149e3b1\#file-success-php" %}

### Info

![](https://vsp.ams3.cdn.digitaloceanspaces.com/sshots/i/2019/Jan/17/1547710026-128.jpg)

{% embed url="https://gist.github.com/wponion-framework/44c457ba6c9cd64a5861a4eb7149e3b1\#file-info-php" %}

### Warning

![](https://vsp.ams3.cdn.digitaloceanspaces.com/sshots/i/2019/Jan/17/1547710117-18.jpg)

{% embed url="https://gist.github.com/wponion-framework/44c457ba6c9cd64a5861a4eb7149e3b1\#file-warning-php" %}

### Error

![](https://vsp.ams3.cdn.digitaloceanspaces.com/sshots/i/2019/Jan/17/1547710171-197.jpg)

{% embed url="https://gist.github.com/wponion-framework/44c457ba6c9cd64a5861a4eb7149e3b1\#file-error-php" %}

### Upgrade

![](https://vsp.ams3.cdn.digitaloceanspaces.com/sshots/i/2019/Jan/17/1547710292-131.jpg)

{% embed url="https://gist.github.com/wponion-framework/44c457ba6c9cd64a5861a4eb7149e3b1\#file-upgrade-php" %}



