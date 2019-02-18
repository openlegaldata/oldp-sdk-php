# Swagger\Client\CasesApi

All URIs are relative to *https://de.openlegaldata.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**casesCreate**](CasesApi.md#casesCreate) | **POST** /cases/ | 
[**casesDelete**](CasesApi.md#casesDelete) | **DELETE** /cases/{id}/ | 
[**casesList**](CasesApi.md#casesList) | **GET** /cases/ | 
[**casesPartialUpdate**](CasesApi.md#casesPartialUpdate) | **PATCH** /cases/{id}/ | 
[**casesRead**](CasesApi.md#casesRead) | **GET** /cases/{id}/ | 
[**casesSearchList**](CasesApi.md#casesSearchList) | **GET** /cases/search/ | 
[**casesUpdate**](CasesApi.md#casesUpdate) | **PUT** /cases/{id}/ | 


# **casesCreate**
> \Swagger\Client\Model\ModelCase casesCreate($data)



List view for cases

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CasesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$data = new \Swagger\Client\Model\ModelCase(); // \Swagger\Client\Model\ModelCase | 

try {
    $result = $apiInstance->casesCreate($data);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CasesApi->casesCreate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**\Swagger\Client\Model\ModelCase**](../Model/ModelCase.md)|  |

### Return type

[**\Swagger\Client\Model\ModelCase**](../Model/ModelCase.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **casesDelete**
> casesDelete($id)



List view for cases

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CasesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | A unique integer value identifying this case.

try {
    $apiInstance->casesDelete($id);
} catch (Exception $e) {
    echo 'Exception when calling CasesApi->casesDelete: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this case. |

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **casesList**
> \Swagger\Client\Model\InlineResponse2003 casesList($ordering, $date, $slug, $file_number, $ecli, $court, $court__slug, $court__jurisdiction, $court__level_of_appeal, $court__state, $page, $page_size)



List view for cases

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CasesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$ordering = "ordering_example"; // string | Which field to use when ordering the results.
$date = "date_example"; // string | 
$slug = "slug_example"; // string | 
$file_number = "file_number_example"; // string | 
$ecli = "ecli_example"; // string | 
$court = 8.14; // float | 
$court__slug = "court__slug_example"; // string | 
$court__jurisdiction = "court__jurisdiction_example"; // string | 
$court__level_of_appeal = "court__level_of_appeal_example"; // string | 
$court__state = "court__state_example"; // string | 
$page = 56; // int | A page number within the paginated result set.
$page_size = 56; // int | Number of results to return per page.

try {
    $result = $apiInstance->casesList($ordering, $date, $slug, $file_number, $ecli, $court, $court__slug, $court__jurisdiction, $court__level_of_appeal, $court__state, $page, $page_size);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CasesApi->casesList: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ordering** | **string**| Which field to use when ordering the results. | [optional]
 **date** | **string**|  | [optional]
 **slug** | **string**|  | [optional]
 **file_number** | **string**|  | [optional]
 **ecli** | **string**|  | [optional]
 **court** | **float**|  | [optional]
 **court__slug** | **string**|  | [optional]
 **court__jurisdiction** | **string**|  | [optional]
 **court__level_of_appeal** | **string**|  | [optional]
 **court__state** | **string**|  | [optional]
 **page** | **int**| A page number within the paginated result set. | [optional]
 **page_size** | **int**| Number of results to return per page. | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse2003**](../Model/InlineResponse2003.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **casesPartialUpdate**
> \Swagger\Client\Model\ModelCase casesPartialUpdate($id, $data)



List view for cases

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CasesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | A unique integer value identifying this case.
$data = new \Swagger\Client\Model\ModelCase(); // \Swagger\Client\Model\ModelCase | 

try {
    $result = $apiInstance->casesPartialUpdate($id, $data);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CasesApi->casesPartialUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this case. |
 **data** | [**\Swagger\Client\Model\ModelCase**](../Model/ModelCase.md)|  |

### Return type

[**\Swagger\Client\Model\ModelCase**](../Model/ModelCase.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **casesRead**
> \Swagger\Client\Model\ModelCase casesRead($id)



List view for cases

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CasesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | A unique integer value identifying this case.

try {
    $result = $apiInstance->casesRead($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CasesApi->casesRead: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this case. |

### Return type

[**\Swagger\Client\Model\ModelCase**](../Model/ModelCase.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **casesSearchList**
> \Swagger\Client\Model\InlineResponse2004 casesSearchList($text, $facet_model_name, $date, $court_jurisdiction, $court_level_of_appeal, $decision_type, $court, $page, $page_size)



Search view (list only)

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CasesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$text = "text_example"; // string | Search query on text content (Lucence syntax support).
$facet_model_name = "facet_model_name_example"; // string | facet_model_name
$date = "date_example"; // string | date
$court_jurisdiction = "court_jurisdiction_example"; // string | court_jurisdiction
$court_level_of_appeal = "court_level_of_appeal_example"; // string | court_level_of_appeal
$decision_type = "decision_type_example"; // string | decision_type
$court = "court_example"; // string | court
$page = 56; // int | A page number within the paginated result set.
$page_size = 56; // int | Number of results to return per page.

try {
    $result = $apiInstance->casesSearchList($text, $facet_model_name, $date, $court_jurisdiction, $court_level_of_appeal, $decision_type, $court, $page, $page_size);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CasesApi->casesSearchList: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **text** | **string**| Search query on text content (Lucence syntax support). |
 **facet_model_name** | **string**| facet_model_name | [optional]
 **date** | **string**| date | [optional]
 **court_jurisdiction** | **string**| court_jurisdiction | [optional]
 **court_level_of_appeal** | **string**| court_level_of_appeal | [optional]
 **decision_type** | **string**| decision_type | [optional]
 **court** | **string**| court | [optional]
 **page** | **int**| A page number within the paginated result set. | [optional]
 **page_size** | **int**| Number of results to return per page. | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse2004**](../Model/InlineResponse2004.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **casesUpdate**
> \Swagger\Client\Model\ModelCase casesUpdate($id, $data)



List view for cases

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\CasesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int | A unique integer value identifying this case.
$data = new \Swagger\Client\Model\ModelCase(); // \Swagger\Client\Model\ModelCase | 

try {
    $result = $apiInstance->casesUpdate($id, $data);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CasesApi->casesUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this case. |
 **data** | [**\Swagger\Client\Model\ModelCase**](../Model/ModelCase.md)|  |

### Return type

[**\Swagger\Client\Model\ModelCase**](../Model/ModelCase.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

