JEditable Bundle for Symfony2

## Current Version

JEditable 1.7.3

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
        // ...
        "tuupola/jeditable-bundle": "dev-master"
    }
}
```

### Add bundle to your application kernel

``` php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new Tuupola\JEditableBundle\TuupolaJEditableBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update tuupola/jeditable-bundle
```

### Install assets

Given your server's public directory is named "web", install the public vendor resources

``` bash
$ php app/console assets:install web
```

Optionally, use the --symlink attribute to create links rather than copies of the resources 

``` bash
$ php app/console assets:install --symlink web
```

## Usage

Refer to the desired files in your HTML template, e.g.

``` html
{% javascripts '@TuupolaJEditableBundle/Resources/public/js/jquery.jeditable.min.js' %}
    <script type="text/javascript" src="{{ asset_url }}"></script>
{% endjavascripts %}
```

## Licenses

Refer to the source code of the included files for license information

## References

1. http://www.appelsiini.net/projects/jeditable
2. http://symfony.com
