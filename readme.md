Laravel Recurly Package
=======================

Integrates the Recurly API with Laravel 5.

A simple [Laravel 5](http://laravel.com/) service provider for including the [Recurly PHP Client](https://github.com/recurly/recurly-client-php).

## Installation

Use composer to install the package.
```bash
composer require jorisvanw/laravel-recurly
```
For laravel >=5.5 that's all. This package supports Laravel new Package Discovery.

If you are using Laravel < 5.5, you also need to add 'JorisvanW\LaravelRecurly\ServiceProvider' to your app/config/app.php providers array:
```php
JorisvanW\LaravelRecurly\ServiceProvider::class,
```

## Configuration

The defaults are set in `app/config/recurly.php`. Copy this file to your own config directory to modify the values. You can publish the config using this command:

```sh
$ php artisan vendor:publish --provider="JorisvanW\LaravelRecurly\ServiceProvider"
```

Add your Recurly information to the your .env file using the keys found in `app/config/recurly.php`.

## Usage

http://docs.recurly.com/client-libraries/php
