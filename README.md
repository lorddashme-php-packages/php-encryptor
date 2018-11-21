# PHP Cryptor

A PHP package wrapper for cryptography functions.

[![Latest Stable Version](https://img.shields.io/packagist/v/lorddashme/php-cryptor.svg?style=flat-square)](https://packagist.org/packages/lorddashme/php-cryptor) [![Minimum PHP Version](https://img.shields.io/badge/php-%3E%3D%205.6-8892BF.svg?style=flat-square)](https://php.net/) [![Build Status](https://img.shields.io/travis/LordDashMe/php-cryptor/master.svg?style=flat-square)](https://travis-ci.org/LordDashMe/php-cryptor) [![Coverage Status](https://img.shields.io/coveralls/LordDashMe/php-cryptor/master.svg?style=flat-square)](https://coveralls.io/github/LordDashMe/php-cryptor?branch=master)

## Requirement(s)

- PHP version from 5.6.* up to latest.

## Install

- It is advice to install the package via Composer. Use the command below to install the package:

```txt
composer require lorddashme/php-cryptor
```

## Usage

```php
<?php

include __DIR__  . '/vendor/autoload.php';

use LordDashMe\Cryptor\Cryptor;

$cryptor = new Cryptor(
    Cryptor::METHOD_ALIAS_AES256
);

$cryptor->key('password');
$cryptor->content('this is the plain text');
$cryptor->encrypt(); // YToyOntzOjc6ImNvbnRlbnQiO3M6MzI6Iqu403ErS5CwNfPPN/j8ohvJoZApgcDUvbD70Rm/2TQEIjtzOjI6Iml2IjtzOjE2OiJQOd1Y8AIYy8JDhNsdeh/hIjt9
```

## License

This package is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
