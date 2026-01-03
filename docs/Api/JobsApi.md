# MailSafePro\JobsApi



All URIs are relative to http://localhost, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createJobJobsV1JobsPost()**](JobsApi.md#createJobJobsV1JobsPost) | **POST** /jobs/v1/jobs | Create validation job |
| [**createJobJobsV1JobsPost_0()**](JobsApi.md#createJobJobsV1JobsPost_0) | **POST** /jobs/v1/jobs | Create validation job |
| [**getJobResultsJobsV1JobsJobIdResultsGet()**](JobsApi.md#getJobResultsJobsV1JobsJobIdResultsGet) | **GET** /jobs/v1/jobs/{job_id}/results | Get job results (paged) |
| [**getJobResultsJobsV1JobsJobIdResultsGet_0()**](JobsApi.md#getJobResultsJobsV1JobsJobIdResultsGet_0) | **GET** /jobs/v1/jobs/{job_id}/results | Get job results (paged) |
| [**getJobStatusJobsV1JobsJobIdGet()**](JobsApi.md#getJobStatusJobsV1JobsJobIdGet) | **GET** /jobs/v1/jobs/{job_id} | Get job status |
| [**getJobStatusJobsV1JobsJobIdGet_0()**](JobsApi.md#getJobStatusJobsV1JobsJobIdGet_0) | **GET** /jobs/v1/jobs/{job_id} | Get job status |


## `createJobJobsV1JobsPost()`

```php
createJobJobsV1JobsPost($job_create_request, $x_idempotency_key, $x_api_key, $authorization): \MailSafePro\Model\JobCreateResponse
```

Create validation job

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\JobsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$job_create_request = new \MailSafePro\Model\JobCreateRequest(); // \MailSafePro\Model\JobCreateRequest
$x_idempotency_key = 'x_idempotency_key_example'; // string
$x_api_key = 'x_api_key_example'; // string
$authorization = 'authorization_example'; // string

try {
    $result = $apiInstance->createJobJobsV1JobsPost($job_create_request, $x_idempotency_key, $x_api_key, $authorization);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling JobsApi->createJobJobsV1JobsPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **job_create_request** | [**\MailSafePro\Model\JobCreateRequest**](../Model/JobCreateRequest.md)|  | |
| **x_idempotency_key** | **string**|  | [optional] |
| **x_api_key** | **string**|  | [optional] |
| **authorization** | **string**|  | [optional] |

### Return type

[**\MailSafePro\Model\JobCreateResponse**](../Model/JobCreateResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createJobJobsV1JobsPost_0()`

```php
createJobJobsV1JobsPost_0($job_create_request, $x_idempotency_key, $x_api_key, $authorization): \MailSafePro\Model\JobCreateResponse
```

Create validation job

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\JobsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$job_create_request = new \MailSafePro\Model\JobCreateRequest(); // \MailSafePro\Model\JobCreateRequest
$x_idempotency_key = 'x_idempotency_key_example'; // string
$x_api_key = 'x_api_key_example'; // string
$authorization = 'authorization_example'; // string

try {
    $result = $apiInstance->createJobJobsV1JobsPost_0($job_create_request, $x_idempotency_key, $x_api_key, $authorization);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling JobsApi->createJobJobsV1JobsPost_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **job_create_request** | [**\MailSafePro\Model\JobCreateRequest**](../Model/JobCreateRequest.md)|  | |
| **x_idempotency_key** | **string**|  | [optional] |
| **x_api_key** | **string**|  | [optional] |
| **authorization** | **string**|  | [optional] |

### Return type

[**\MailSafePro\Model\JobCreateResponse**](../Model/JobCreateResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getJobResultsJobsV1JobsJobIdResultsGet()`

```php
getJobResultsJobsV1JobsJobIdResultsGet($job_id, $page, $size, $x_api_key, $authorization): \MailSafePro\Model\JobResultsPage
```

Get job results (paged)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\JobsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$job_id = 'job_id_example'; // string
$page = 1; // int
$size = 500; // int
$x_api_key = 'x_api_key_example'; // string
$authorization = 'authorization_example'; // string

try {
    $result = $apiInstance->getJobResultsJobsV1JobsJobIdResultsGet($job_id, $page, $size, $x_api_key, $authorization);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling JobsApi->getJobResultsJobsV1JobsJobIdResultsGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **job_id** | **string**|  | |
| **page** | **int**|  | [optional] [default to 1] |
| **size** | **int**|  | [optional] [default to 500] |
| **x_api_key** | **string**|  | [optional] |
| **authorization** | **string**|  | [optional] |

### Return type

[**\MailSafePro\Model\JobResultsPage**](../Model/JobResultsPage.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getJobResultsJobsV1JobsJobIdResultsGet_0()`

```php
getJobResultsJobsV1JobsJobIdResultsGet_0($job_id, $page, $size, $x_api_key, $authorization): \MailSafePro\Model\JobResultsPage
```

Get job results (paged)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\JobsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$job_id = 'job_id_example'; // string
$page = 1; // int
$size = 500; // int
$x_api_key = 'x_api_key_example'; // string
$authorization = 'authorization_example'; // string

try {
    $result = $apiInstance->getJobResultsJobsV1JobsJobIdResultsGet_0($job_id, $page, $size, $x_api_key, $authorization);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling JobsApi->getJobResultsJobsV1JobsJobIdResultsGet_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **job_id** | **string**|  | |
| **page** | **int**|  | [optional] [default to 1] |
| **size** | **int**|  | [optional] [default to 500] |
| **x_api_key** | **string**|  | [optional] |
| **authorization** | **string**|  | [optional] |

### Return type

[**\MailSafePro\Model\JobResultsPage**](../Model/JobResultsPage.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getJobStatusJobsV1JobsJobIdGet()`

```php
getJobStatusJobsV1JobsJobIdGet($job_id, $x_api_key, $authorization): \MailSafePro\Model\JobStatusResponse
```

Get job status

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\JobsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$job_id = 'job_id_example'; // string
$x_api_key = 'x_api_key_example'; // string
$authorization = 'authorization_example'; // string

try {
    $result = $apiInstance->getJobStatusJobsV1JobsJobIdGet($job_id, $x_api_key, $authorization);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling JobsApi->getJobStatusJobsV1JobsJobIdGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **job_id** | **string**|  | |
| **x_api_key** | **string**|  | [optional] |
| **authorization** | **string**|  | [optional] |

### Return type

[**\MailSafePro\Model\JobStatusResponse**](../Model/JobStatusResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getJobStatusJobsV1JobsJobIdGet_0()`

```php
getJobStatusJobsV1JobsJobIdGet_0($job_id, $x_api_key, $authorization): \MailSafePro\Model\JobStatusResponse
```

Get job status

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\JobsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$job_id = 'job_id_example'; // string
$x_api_key = 'x_api_key_example'; // string
$authorization = 'authorization_example'; // string

try {
    $result = $apiInstance->getJobStatusJobsV1JobsJobIdGet_0($job_id, $x_api_key, $authorization);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling JobsApi->getJobStatusJobsV1JobsJobIdGet_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **job_id** | **string**|  | |
| **x_api_key** | **string**|  | [optional] |
| **authorization** | **string**|  | [optional] |

### Return type

[**\MailSafePro\Model\JobStatusResponse**](../Model/JobStatusResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
