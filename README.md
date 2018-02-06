# Basic Authentication handler for the JSON API
* Download the plugin into your plugins directory
* Enable in the WordPress admin
## cURL
>curl --user admin:password https://example.com/wp-json/

## PHP
```php
$args = array(
	'headers' => array(
		'Authorization' => 'Basic ' . base64_encode( $username . ':' . $password ),
	),
);
