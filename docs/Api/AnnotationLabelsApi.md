# Swagger\Client\AnnotationLabelsApi

All URIs are relative to *https://de.openlegaldata.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**annotationLabelsCreate**](AnnotationLabelsApi.md#annotationLabelsCreate) | **POST** /annotation_labels/ | 
[**annotationLabelsDelete**](AnnotationLabelsApi.md#annotationLabelsDelete) | **DELETE** /annotation_labels/{id}/ | 
[**annotationLabelsList**](AnnotationLabelsApi.md#annotationLabelsList) | **GET** /annotation_labels/ | 
[**annotationLabelsPartialUpdate**](AnnotationLabelsApi.md#annotationLabelsPartialUpdate) | **PATCH** /annotation_labels/{id}/ | 
[**annotationLabelsRead**](AnnotationLabelsApi.md#annotationLabelsRead) | **GET** /annotation_labels/{id}/ | 
[**annotationLabelsUpdate**](AnnotationLabelsApi.md#annotationLabelsUpdate) | **PUT** /annotation_labels/{id}/ | 


# **annotationLabelsCreate**
> \Swagger\Client\Model\AnnotationLabel annotationLabelsCreate($data)





### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\AnnotationLabelsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$data = new \Swagger\Client\Model\AnnotationLabel(); // \Swagger\Client\Model\AnnotationLabel | 

try {
    $result = $apiInstance->annotationLabelsCreate($data);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AnnotationLabelsApi->annotationLabelsCreate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**\Swagger\Client\Model\AnnotationLabel**](../Model/AnnotationLabel.md)|  |

### Return type

[**\Swagger\Client\Model\AnnotationLabel**](../Model/AnnotationLabel.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **annotationLabelsDelete**
> annotationLabelsDelete($id)





### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\AnnotationLabelsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | A unique integer value identifying this Label.

try {
    $apiInstance->annotationLabelsDelete($id);
} catch (Exception $e) {
    echo 'Exception when calling AnnotationLabelsApi->annotationLabelsDelete: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this Label. |

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **annotationLabelsList**
> \Swagger\Client\Model\InlineResponse200 annotationLabelsList($ordering, $owner, $slug, $private, $trusted, $limit, $offset)





### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\AnnotationLabelsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$ordering = "ordering_example"; // string | Which field to use when ordering the results.
$owner = 8.14; // float | 
$slug = "slug_example"; // string | 
$private = "private_example"; // string | 
$trusted = "trusted_example"; // string | 
$limit = 56; // int | Number of results to return per page.
$offset = 56; // int | The initial index from which to return the results.

try {
    $result = $apiInstance->annotationLabelsList($ordering, $owner, $slug, $private, $trusted, $limit, $offset);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AnnotationLabelsApi->annotationLabelsList: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ordering** | **string**| Which field to use when ordering the results. | [optional]
 **owner** | **float**|  | [optional]
 **slug** | **string**|  | [optional]
 **private** | **string**|  | [optional]
 **trusted** | **string**|  | [optional]
 **limit** | **int**| Number of results to return per page. | [optional]
 **offset** | **int**| The initial index from which to return the results. | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse200**](../Model/InlineResponse200.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **annotationLabelsPartialUpdate**
> \Swagger\Client\Model\AnnotationLabel annotationLabelsPartialUpdate($id, $data)





### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\AnnotationLabelsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | A unique integer value identifying this Label.
$data = new \Swagger\Client\Model\AnnotationLabel(); // \Swagger\Client\Model\AnnotationLabel | 

try {
    $result = $apiInstance->annotationLabelsPartialUpdate($id, $data);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AnnotationLabelsApi->annotationLabelsPartialUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this Label. |
 **data** | [**\Swagger\Client\Model\AnnotationLabel**](../Model/AnnotationLabel.md)|  |

### Return type

[**\Swagger\Client\Model\AnnotationLabel**](../Model/AnnotationLabel.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **annotationLabelsRead**
> \Swagger\Client\Model\AnnotationLabel annotationLabelsRead($id)





### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\AnnotationLabelsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | A unique integer value identifying this Label.

try {
    $result = $apiInstance->annotationLabelsRead($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AnnotationLabelsApi->annotationLabelsRead: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this Label. |

### Return type

[**\Swagger\Client\Model\AnnotationLabel**](../Model/AnnotationLabel.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **annotationLabelsUpdate**
> \Swagger\Client\Model\AnnotationLabel annotationLabelsUpdate($id, $data)





### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\AnnotationLabelsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | A unique integer value identifying this Label.
$data = new \Swagger\Client\Model\AnnotationLabel(); // \Swagger\Client\Model\AnnotationLabel | 

try {
    $result = $apiInstance->annotationLabelsUpdate($id, $data);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AnnotationLabelsApi->annotationLabelsUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this Label. |
 **data** | [**\Swagger\Client\Model\AnnotationLabel**](../Model/AnnotationLabel.md)|  |

### Return type

[**\Swagger\Client\Model\AnnotationLabel**](../Model/AnnotationLabel.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

