# WordPress API Client

This is a PHP client for the [WordPress JSON REST API](https://github.com/WP-API/WP-API). It's designed to work with WordPress
without the need for an external library. This is done by leveraging the [WordPress HTTP API](http://codex.wordpress.org/HTTP_API) through
the `WP_Http`class.

## Background

The client was created as part of an [article](http://carlalexander.ca/designing-class-wordpress-api-client) on how to design a class.

## Current limitations

This is still a work in progress. The client currently only supports the `get_users` method. You can also only authenticate using
[basic authentication](https://github.com/WP-API/Basic-Auth).

## Usage

```php
$client = GV_API_Client::create('http://your.wordpress.org', 'your_token');

$users = $client->get_users();
```

## Bugs

For bugs or feature requests, please [create an issue](https://github.com/carlalexander/wp-api-client/issues/new).