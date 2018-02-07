# SayWhenNachonUtils\FilterApi

All URIs are relative to *https://link.saywhen.nl/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getDeliveryFloor**](FilterApi.md#getDeliveryFloor) | **POST** /nachon/utils/get-delivery-floor | GetDeliveryFloor from SurveyResults


# **getDeliveryFloor**
> \SayWhenNachonUtils\Model\ApiResponse getDeliveryFloor($body)

GetDeliveryFloor from SurveyResults

GetDeliveryFloor from SurveyResults

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
SayWhenNachonUtils\Configuration::getDefaultConfiguration()->setApiKey('ApiKey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// SayWhenNachonUtils\Configuration::getDefaultConfiguration()->setApiKeyPrefix('ApiKey', 'Bearer');

$api_instance = new SayWhenNachonUtils\Api\FilterApi();
$body = new \SayWhenNachonUtils\Model\GetDeliveryFloorModelPostModel(); // \SayWhenNachonUtils\Model\GetDeliveryFloorModelPostModel | GetDeliveryFloorModelPostModel

try {
    $result = $api_instance->getDeliveryFloor($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling FilterApi->getDeliveryFloor: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\SayWhenNachonUtils\Model\GetDeliveryFloorModelPostModel**](../Model/GetDeliveryFloorModelPostModel.md)| GetDeliveryFloorModelPostModel |

### Return type

[**\SayWhenNachonUtils\Model\ApiResponse**](../Model/ApiResponse.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json, application/xml
 - **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

