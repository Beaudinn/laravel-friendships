# Laravel Friendships [![Build Status](https://travis-ci.org/hootlex/laravel-friendships.svg?branch=master)](https://travis-ci.org/hootlex/laravel-friendships)

This package gives Eloqent models the ability to manage their friendships.
###Models can:
- Send Friend Requests
- Accept Friend Requests
- Deny Friend Requests
- Block Another Model

## Installation

First, install the package through Composer.

```php
composer require hootlex/laravel-friendships
```

Then include the service provider inside `config/app.php`.

```php
'providers' => [
    ...
    Hootlex\Friendships\FriendshipsServiceProvider::class,
    ...
];
```
Lastly you need to publish the migration and migrate the database

```
php artisan vendor:publish --provider="Hootlex\Friendships\FriendshipsServiceProvider" && artisan migrate
```
