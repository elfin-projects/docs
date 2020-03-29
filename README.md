---
description: Example markdown syntax for gitbook
---

# EXAMPLE REFS

### task list

* [ ] task1
* [ ] task2

### code block

{% code title="test.cpp" %}
```cpp
// this is a code block with file name
```
{% endcode %}

### hint box

{% hint style="info" %}
This is a hint
{% endhint %}

### block link

{% page-ref page="another-group/in-group-page.md" %}

### attachment

{% file src=".gitbook/assets/magical-mirai.jpeg" caption="This is a file" %}

### equation

$$
a = b
$$

### tab

{% tabs %}
{% tab title="First Tab" %}
First Tab content
{% endtab %}

{% tab title="Second Tab" %}
Second Tab content
{% endtab %}
{% endtabs %}

### api

{% api-method method="get" host="https://example.com" path="/v1/example" %}
{% api-method-summary %}
Test API METHOD
{% endapi-method-summary %}

{% api-method-description %}
description for api
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="path-param" type="string" required=true %}
description
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="header-param" type="string" required=false %}
description
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% api-method-parameter name="query-param" type="string" required=false %}
description
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}

{% api-method-form-data-parameters %}
{% api-method-parameter name="form-data" type="string" required=false %}
description
{% endapi-method-parameter %}
{% endapi-method-form-data-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="body-param" type="string" required=false %}
description
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
All fine
{% endapi-method-response-example-description %}

```javascript
{
    "status": "ok"
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=500 %}
{% api-method-response-example-description %}
Just error
{% endapi-method-response-example-description %}

```
NO CONTENT
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



