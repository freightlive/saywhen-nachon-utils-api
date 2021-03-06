# 
SayWhen Utils for Nachon API Documentation

This PHP package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: 1.0
- Build package: io.swagger.codegen.languages.PhpClientCodegen

## Requirements

PHP 5.4.0 and later

## Installation & Usage
### Composer

To install the bindings via [Composer](http://getcomposer.org/), add the following to `composer.json`:

```
{
  "repositories": [
    {
      "type": "git",
      "url": "https://github.com/bumbal/saywhen-nachon-utils-api.git"
    }
  ],
  "require": {
    "bumbal/saywhen-nachon-utils-api": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to//autoload.php');
```

## Tests

To run the unit tests:

```
composer install
./vendor/bin/phpunit
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
SayWhenNachonUtils\Configuration::getDefaultConfiguration()->setApiKey('ApiKey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// SayWhenNachonUtils\Configuration::getDefaultConfiguration()->setApiKeyPrefix('ApiKey', 'Bearer');

$api_instance = new SayWhenNachonUtils\Api\UtilsApi();
$body = new \SayWhenNachonUtils\Model\GetDeliveryFloorModelPostModel(); // \SayWhenNachonUtils\Model\GetDeliveryFloorModelPostModel | GetDeliveryFloorModelPostModel

try {
    $result = $api_instance->getDeliveryFloor($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UtilsApi->getDeliveryFloor: ', $e->getMessage(), PHP_EOL;
}

?>
```

## Documentation for API Endpoints

All URIs are relative to *https://link.saywhen.nl/api/v1*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*UtilsApi* | [**getDeliveryFloor**](docs/Api/UtilsApi.md#getdeliveryfloor) | **POST** /nachon/utils/get-delivery-floor | GetDeliveryFloor from SurveyResults


## Documentation For Models

 - [ApiResponse](docs/Model/ApiResponse.md)
 - [GetDeliveryFloorModelPostModel](docs/Model/GetDeliveryFloorModelPostModel.md)


## Documentation For Authorization


## api_key

- **Type**: API key
- **API key parameter name**: ApiKey
- **Location**: HTTP header


## Author

gerb@bumbal.eu


