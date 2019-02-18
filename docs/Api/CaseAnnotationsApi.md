# Swagger\Client\CaseAnnotationsApi

All URIs are relative to *https://de.openlegaldata.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**caseAnnotationsCreate**](CaseAnnotationsApi.md#caseAnnotationsCreate) | **POST** /case_annotations/ | 
[**caseAnnotationsDelete**](CaseAnnotationsApi.md#caseAnnotationsDelete) | **DELETE** /case_annotations/{id}/ | 
[**caseAnnotationsList**](CaseAnnotationsApi.md#caseAnnotationsList) | **GET** /case_annotations/ | 
[**caseAnnotationsPartialUpdate**](CaseAnnotationsApi.md#caseAnnotationsPartialUpdate) | **PATCH** /case_annotations/{id}/ | 
[**caseAnnotationsRead**](CaseAnnotationsApi.md#caseAnnotationsRead) | **GET** /case_annotations/{id}/ | 
[**caseAnnotationsUpdate**](CaseAnnotationsApi.md#caseAnnotationsUpdate) | **PUT** /case_annotations/{id}/ | 


# **caseAnnotationsCreate**
> \Swagger\Client\Model\CaseAnnotation caseAnnotationsCreate($data)





### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CaseAnnotationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$data = new \Swagger\Client\Model\CaseAnnotation(); // \Swagger\Client\Model\CaseAnnotation | 

try {
    $result = $apiInstance->caseAnnotationsCreate($data);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CaseAnnotationsApi->caseAnnotationsCreate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**\Swagger\Client\Model\CaseAnnotation**](../Model/CaseAnnotation.md)|  |

### Return type

[**\Swagger\Client\Model\CaseAnnotation**](../Model/CaseAnnotation.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **caseAnnotationsDelete**
> caseAnnotationsDelete($id)





### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CaseAnnotationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | A unique integer value identifying this case annotation.

try {
    $apiInstance->caseAnnotationsDelete($id);
} catch (Exception $e) {
    echo 'Exception when calling CaseAnnotationsApi->caseAnnotationsDelete: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this case annotation. |

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **caseAnnotationsList**
> \Swagger\Client\Model\InlineResponse2001 caseAnnotationsList($belongs_to, $label, $limit, $offset)





### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CaseAnnotationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$belongs_to = 8.14; // float | 
$label = 8.14; // float | 
$limit = 56; // int | Number of results to return per page.
$offset = 56; // int | The initial index from which to return the results.

try {
    $result = $apiInstance->caseAnnotationsList($belongs_to, $label, $limit, $offset);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CaseAnnotationsApi->caseAnnotationsList: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **belongs_to** | **float**|  | [optional]
 **label** | **float**|  | [optional]
 **limit** | **int**| Number of results to return per page. | [optional]
 **offset** | **int**| The initial index from which to return the results. | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse2001**](../Model/InlineResponse2001.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **caseAnnotationsPartialUpdate**
> \Swagger\Client\Model\CaseAnnotation caseAnnotationsPartialUpdate($id, $data)





### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CaseAnnotationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | A unique integer value identifying this case annotation.
$data = new \Swagger\Client\Model\CaseAnnotation(); // \Swagger\Client\Model\CaseAnnotation | 

try {
    $result = $apiInstance->caseAnnotationsPartialUpdate($id, $data);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CaseAnnotationsApi->caseAnnotationsPartialUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this case annotation. |
 **data** | [**\Swagger\Client\Model\CaseAnnotation**](../Model/CaseAnnotation.md)|  |

### Return type

[**\Swagger\Client\Model\CaseAnnotation**](../Model/CaseAnnotation.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **caseAnnotationsRead**
> \Swagger\Client\Model\CaseAnnotation caseAnnotationsRead($id)





### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CaseAnnotationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | A unique integer value identifying this case annotation.

try {
    $result = $apiInstance->caseAnnotationsRead($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CaseAnnotationsApi->caseAnnotationsRead: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this case annotation. |

### Return type

[**\Swagger\Client\Model\CaseAnnotation**](../Model/CaseAnnotation.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **caseAnnotationsUpdate**
> \Swagger\Client\Model\CaseAnnotation caseAnnotationsUpdate($id, $data)





### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CaseAnnotationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | A unique integer value identifying this case annotation.
$data = new \Swagger\Client\Model\CaseAnnotation(); // \Swagger\Client\Model\CaseAnnotation | 

try {
    $result = $apiInstance->caseAnnotationsUpdate($id, $data);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CaseAnnotationsApi->caseAnnotationsUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this case annotation. |
 **data** | [**\Swagger\Client\Model\CaseAnnotation**](../Model/CaseAnnotation.md)|  |

### Return type

[**\Swagger\Client\Model\CaseAnnotation**](../Model/CaseAnnotation.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

