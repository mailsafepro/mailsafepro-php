# MailSafePro\LogsApi



All URIs are relative to http://localhost, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**clearRequestLogsLogsLogsRequestsDelete()**](LogsApi.md#clearRequestLogsLogsLogsRequestsDelete) | **DELETE** /logs/logs/requests | Clear Request Logs |
| [**getRequestLogsLogsLogsRequestsGet()**](LogsApi.md#getRequestLogsLogsLogsRequestsGet) | **GET** /logs/logs/requests | Get Request Logs |


## `clearRequestLogsLogsLogsRequestsDelete()`

```php
clearRequestLogsLogsLogsRequestsDelete(): mixed
```

Clear Request Logs

Clear all request logs for current user.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\LogsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->clearRequestLogsLogsLogsRequestsDelete();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling LogsApi->clearRequestLogsLogsLogsRequestsDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

**mixed**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getRequestLogsLogsLogsRequestsGet()`

```php
getRequestLogsLogsLogsRequestsGet($limit, $status_code, $endpoint, $method, $since): mixed
```

Get Request Logs

Get request logs for authenticated user.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\LogsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$limit = 100; // int | Max results to return
$status_code = 56; // int | Filter by HTTP status code
$endpoint = 'endpoint_example'; // string | Filter by endpoint path
$method = 'method_example'; // string | Filter by HTTP method (GET, POST, etc)
$since = new \DateTime('2013-10-20T19:20:30+01:00'); // \DateTime | Filter by timestamp (ISO 8601)

try {
    $result = $apiInstance->getRequestLogsLogsLogsRequestsGet($limit, $status_code, $endpoint, $method, $since);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling LogsApi->getRequestLogsLogsLogsRequestsGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **int**| Max results to return | [optional] [default to 100] |
| **status_code** | **int**| Filter by HTTP status code | [optional] |
| **endpoint** | **string**| Filter by endpoint path | [optional] |
| **method** | **string**| Filter by HTTP method (GET, POST, etc) | [optional] |
| **since** | **\DateTime**| Filter by timestamp (ISO 8601) | [optional] |

### Return type

**mixed**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
