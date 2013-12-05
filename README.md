Lo-Dash Bundle for Symfony2

## Current Version

Lo-Dash v2.4.1

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "bmatzner/lodash-bundle": "~2.4"
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
        new Bmatzner\LoDashBundle\BmatznerLoDashBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update bmatzner/lodash-bundle
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
<script type="text/javascript" src="{{ asset('bundles/bmatznerlodash/js/lodash.min.js') }}"></script>
```

## Licenses

Refer to the source code of the included files for license information

## References

1. http://lodash.com/
2. http://symfony.com/
