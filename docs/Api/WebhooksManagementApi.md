# MailSafePro\WebhooksManagementApi



All URIs are relative to http://localhost, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createWebhookWebhooksManagementWebhooksPost()**](WebhooksManagementApi.md#createWebhookWebhooksManagementWebhooksPost) | **POST** /webhooks-management/webhooks/ | Create Webhook |
| [**deleteWebhookWebhooksManagementWebhooksWebhookIdDelete()**](WebhooksManagementApi.md#deleteWebhookWebhooksManagementWebhooksWebhookIdDelete) | **DELETE** /webhooks-management/webhooks/{webhook_id} | Delete Webhook |
| [**getDeliveriesWebhooksManagementWebhooksWebhookIdDeliveriesGet()**](WebhooksManagementApi.md#getDeliveriesWebhooksManagementWebhooksWebhookIdDeliveriesGet) | **GET** /webhooks-management/webhooks/{webhook_id}/deliveries | Get Deliveries |
| [**getWebhookWebhooksManagementWebhooksWebhookIdGet()**](WebhooksManagementApi.md#getWebhookWebhooksManagementWebhooksWebhookIdGet) | **GET** /webhooks-management/webhooks/{webhook_id} | Get Webhook |
| [**listWebhooksWebhooksManagementWebhooksGet()**](WebhooksManagementApi.md#listWebhooksWebhooksManagementWebhooksGet) | **GET** /webhooks-management/webhooks/ | List Webhooks |
| [**testWebhookWebhooksManagementWebhooksWebhookIdTestPost()**](WebhooksManagementApi.md#testWebhookWebhooksManagementWebhooksWebhookIdTestPost) | **POST** /webhooks-management/webhooks/{webhook_id}/test | Test Webhook |
| [**updateWebhookWebhooksManagementWebhooksWebhookIdPatch()**](WebhooksManagementApi.md#updateWebhookWebhooksManagementWebhooksWebhookIdPatch) | **PATCH** /webhooks-management/webhooks/{webhook_id} | Update Webhook |


## `createWebhookWebhooksManagementWebhooksPost()`

```php
createWebhookWebhooksManagementWebhooksPost($webhook_create): mixed
```

Create Webhook

Create a new webhook endpoint.  Events available: - validation.completed: Single email validation finished - batch.completed: Batch validation finished - usage.limit_reached: API usage limit reached (80%)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\WebhooksManagementApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$webhook_create = new \MailSafePro\Model\WebhookCreate(); // \MailSafePro\Model\WebhookCreate

try {
    $result = $apiInstance->createWebhookWebhooksManagementWebhooksPost($webhook_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling WebhooksManagementApi->createWebhookWebhooksManagementWebhooksPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **webhook_create** | [**\MailSafePro\Model\WebhookCreate**](../Model/WebhookCreate.md)|  | |

### Return type

**mixed**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deleteWebhookWebhooksManagementWebhooksWebhookIdDelete()`

```php
deleteWebhookWebhooksManagementWebhooksWebhookIdDelete($webhook_id): mixed
```

Delete Webhook

Delete webhook.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\WebhooksManagementApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$webhook_id = 'webhook_id_example'; // string

try {
    $result = $apiInstance->deleteWebhookWebhooksManagementWebhooksWebhookIdDelete($webhook_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling WebhooksManagementApi->deleteWebhookWebhooksManagementWebhooksWebhookIdDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **webhook_id** | **string**|  | |

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

## `getDeliveriesWebhooksManagementWebhooksWebhookIdDeliveriesGet()`

```php
getDeliveriesWebhooksManagementWebhooksWebhookIdDeliveriesGet($webhook_id, $limit): mixed
```

Get Deliveries

Get delivery history for webhook.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\WebhooksManagementApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$webhook_id = 'webhook_id_example'; // string
$limit = 100; // int

try {
    $result = $apiInstance->getDeliveriesWebhooksManagementWebhooksWebhookIdDeliveriesGet($webhook_id, $limit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling WebhooksManagementApi->getDeliveriesWebhooksManagementWebhooksWebhookIdDeliveriesGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **webhook_id** | **string**|  | |
| **limit** | **int**|  | [optional] [default to 100] |

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

## `getWebhookWebhooksManagementWebhooksWebhookIdGet()`

```php
getWebhookWebhooksManagementWebhooksWebhookIdGet($webhook_id): mixed
```

Get Webhook

Get webhook details.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\WebhooksManagementApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$webhook_id = 'webhook_id_example'; // string

try {
    $result = $apiInstance->getWebhookWebhooksManagementWebhooksWebhookIdGet($webhook_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling WebhooksManagementApi->getWebhookWebhooksManagementWebhooksWebhookIdGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **webhook_id** | **string**|  | |

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

## `listWebhooksWebhooksManagementWebhooksGet()`

```php
listWebhooksWebhooksManagementWebhooksGet(): mixed
```

List Webhooks

List all webhooks for authenticated user.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\WebhooksManagementApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->listWebhooksWebhooksManagementWebhooksGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling WebhooksManagementApi->listWebhooksWebhooksManagementWebhooksGet: ', $e->getMessage(), PHP_EOL;
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

## `testWebhookWebhooksManagementWebhooksWebhookIdTestPost()`

```php
testWebhookWebhooksManagementWebhooksWebhookIdTestPost($webhook_id): mixed
```

Test Webhook

Send test event to webhook.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\WebhooksManagementApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$webhook_id = 'webhook_id_example'; // string

try {
    $result = $apiInstance->testWebhookWebhooksManagementWebhooksWebhookIdTestPost($webhook_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling WebhooksManagementApi->testWebhookWebhooksManagementWebhooksWebhookIdTestPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **webhook_id** | **string**|  | |

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

## `updateWebhookWebhooksManagementWebhooksWebhookIdPatch()`

```php
updateWebhookWebhooksManagementWebhooksWebhookIdPatch($webhook_id, $webhook_update): mixed
```

Update Webhook

Update webhook configuration.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\WebhooksManagementApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$webhook_id = 'webhook_id_example'; // string
$webhook_update = new \MailSafePro\Model\WebhookUpdate(); // \MailSafePro\Model\WebhookUpdate

try {
    $result = $apiInstance->updateWebhookWebhooksManagementWebhooksWebhookIdPatch($webhook_id, $webhook_update);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling WebhooksManagementApi->updateWebhookWebhooksManagementWebhooksWebhookIdPatch: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **webhook_id** | **string**|  | |
| **webhook_update** | [**\MailSafePro\Model\WebhookUpdate**](../Model/WebhookUpdate.md)|  | |

### Return type

**mixed**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
