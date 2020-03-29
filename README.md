---
description: Introduction for elfin projects.
---

# ELFIN PROJECTS

Read in：中文 \| English

## Introduction

elfin projects is a php/swoole cored toolkit help you build web apps quickly, without losing much performance.

## Key Features

{% tabs %}
{% tab title="Installation" %}
You can install elfin by using composer.

```bash
composer require elfin/elfin
```

Then just boot the app.

```php
use Elfin\Elfin;
$app = new Elfin();
$app->run();
```
{% endtab %}

{% tab title="Load Services" %}
Suppose you want to create a webapp and using `SomeService` provided by `SomePackage`

```php
use Elfin\Elfin;
use SomePackage\SomeService;

$app = new Elfin();
$app->use(SomeService::class);
$app->run();
```
{% endtab %}

{% tab title="Router" %}
All components are designed to be a `Service`, suppose you want to build a web app using a `Router` or request dispatcher

```php
use Elfin\Elfin;
use Elfin\Support\Router;

$app = new Elfin();
$app->use(Router::class);

// router provided by Elfin\Support\Router
$router = $app->router;
$router->get('/', function ($request, $response) {
    return $response->write('Hello World');
});

$app->run();
```
{% endtab %}
{% endtabs %}

