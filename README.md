**Inverse seed generator (iSeed)** is a Laravel Lumen package that provides a method to generate a new seed file based on data from the existing database table.
This project is based on [orangehill/iseed](https://github.com/orangehill/iseed), all credits to them.

## Installation

### 1. Require with [Composer](https://getcomposer.org/)
```sh
composer require creative-collisions-limited/iseed
```


### 2. Add Service Provider
```php
// '/bootstrap/app.php'
$app->register(CreativeCollisionsLimited\Iseed\IseedServiceProvider::class);
```

## Artisan command options

### [table_name]
Mandatory parameter which defines which table/s will be used for seed creation.
Use CSV notation for multiple tables. Seed file will be generated for each table.

Examples:
```
php artisan iseed my_table
```
```
php artisan iseed my_table,another_table
```
