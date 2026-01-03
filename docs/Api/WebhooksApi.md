# MailSafePro\WebhooksApi



All URIs are relative to http://localhost, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createWebhookWebhooksManagementWebhooksPost()**](WebhooksApi.md#createWebhookWebhooksManagementWebhooksPost) | **POST** /webhooks-management/webhooks/ | Create Webhook |
| [**deleteWebhookWebhooksManagementWebhooksWebhookIdDelete()**](WebhooksApi.md#deleteWebhookWebhooksManagementWebhooksWebhookIdDelete) | **DELETE** /webhooks-management/webhooks/{webhook_id} | Delete Webhook |
| [**getDeliveriesWebhooksManagementWebhooksWebhookIdDeliveriesGet()**](WebhooksApi.md#getDeliveriesWebhooksManagementWebhooksWebhookIdDeliveriesGet) | **GET** /webhooks-management/webhooks/{webhook_id}/deliveries | Get Deliveries |
| [**getWebhookWebhooksManagementWebhooksWebhookIdGet()**](WebhooksApi.md#getWebhookWebhooksManagementWebhooksWebhookIdGet) | **GET** /webhooks-management/webhooks/{webhook_id} | Get Webhook |
| [**listWebhooksWebhooksManagementWebhooksGet()**](WebhooksApi.md#listWebhooksWebhooksManagementWebhooksGet) | **GET** /webhooks-management/webhooks/ | List Webhooks |
| [**registerEndpointWebhooksV1WebhooksEndpointsRegisterPost()**](WebhooksApi.md#registerEndpointWebhooksV1WebhooksEndpointsRegisterPost) | **POST** /webhooks/v1/webhooks/endpoints/register | Register Endpoint |
| [**registerEndpointWebhooksV1WebhooksEndpointsRegisterPost_0()**](WebhooksApi.md#registerEndpointWebhooksV1WebhooksEndpointsRegisterPost_0) | **POST** /webhooks/v1/webhooks/endpoints/register | Register Endpoint |
| [**rotateSecretWebhooksV1WebhooksEndpointsRotatePost()**](WebhooksApi.md#rotateSecretWebhooksV1WebhooksEndpointsRotatePost) | **POST** /webhooks/v1/webhooks/endpoints/rotate | Rotate Secret |
| [**rotateSecretWebhooksV1WebhooksEndpointsRotatePost_0()**](WebhooksApi.md#rotateSecretWebhooksV1WebhooksEndpointsRotatePost_0) | **POST** /webhooks/v1/webhooks/endpoints/rotate | Rotate Secret |
| [**testWebhookWebhooksManagementWebhooksWebhookIdTestPost()**](WebhooksApi.md#testWebhookWebhooksManagementWebhooksWebhookIdTestPost) | **POST** /webhooks-management/webhooks/{webhook_id}/test | Test Webhook |
| [**updateWebhookWebhooksManagementWebhooksWebhookIdPatch()**](WebhooksApi.md#updateWebhookWebhooksManagementWebhooksWebhookIdPatch) | **PATCH** /webhooks-management/webhooks/{webhook_id} | Update Webhook |


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


$apiInstance = new MailSafePro\Api\WebhooksApi(
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
    echo 'Exception when calling WebhooksApi->createWebhookWebhooksManagementWebhooksPost: ', $e->getMessage(), PHP_EOL;
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


$apiInstance = new MailSafePro\Api\WebhooksApi(
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
    echo 'Exception when calling WebhooksApi->deleteWebhookWebhooksManagementWebhooksWebhookIdDelete: ', $e->getMessage(), PHP_EOL;
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


$apiInstance = new MailSafePro\Api\WebhooksApi(
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
    echo 'Exception when calling WebhooksApi->getDeliveriesWebhooksManagementWebhooksWebhookIdDeliveriesGet: ', $e->getMessage(), PHP_EOL;
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


$apiInstance = new MailSafePro\Api\WebhooksApi(
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
    echo 'Exception when calling WebhooksApi->getWebhookWebhooksManagementWebhooksWebhookIdGet: ', $e->getMessage(), PHP_EOL;
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


$apiInstance = new MailSafePro\Api\WebhooksApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->listWebhooksWebhooksManagementWebhooksGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling WebhooksApi->listWebhooksWebhooksManagementWebhooksGet: ', $e->getMessage(), PHP_EOL;
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

## `registerEndpointWebhooksV1WebhooksEndpointsRegisterPost()`

```php
registerEndpointWebhooksV1WebhooksEndpointsRegisterPost($register_endpoint, $x_api_key, $authorization): mixed
```

Register Endpoint

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\WebhooksApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$register_endpoint = new \MailSafePro\Model\RegisterEndpoint(); // \MailSafePro\Model\RegisterEndpoint
$x_api_key = 'x_api_key_example'; // string
$authorization = 'authorization_example'; // string

try {
    $result = $apiInstance->registerEndpointWebhooksV1WebhooksEndpointsRegisterPost($register_endpoint, $x_api_key, $authorization);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling WebhooksApi->registerEndpointWebhooksV1WebhooksEndpointsRegisterPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **register_endpoint** | [**\MailSafePro\Model\RegisterEndpoint**](../Model/RegisterEndpoint.md)|  | |
| **x_api_key** | **string**|  | [optional] |
| **authorization** | **string**|  | [optional] |

### Return type

**mixed**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `registerEndpointWebhooksV1WebhooksEndpointsRegisterPost_0()`

```php
registerEndpointWebhooksV1WebhooksEndpointsRegisterPost_0($register_endpoint, $x_api_key, $authorization): mixed
```

Register Endpoint

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\WebhooksApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$register_endpoint = new \MailSafePro\Model\RegisterEndpoint(); // \MailSafePro\Model\RegisterEndpoint
$x_api_key = 'x_api_key_example'; // string
$authorization = 'authorization_example'; // string

try {
    $result = $apiInstance->registerEndpointWebhooksV1WebhooksEndpointsRegisterPost_0($register_endpoint, $x_api_key, $authorization);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling WebhooksApi->registerEndpointWebhooksV1WebhooksEndpointsRegisterPost_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **register_endpoint** | [**\MailSafePro\Model\RegisterEndpoint**](../Model/RegisterEndpoint.md)|  | |
| **x_api_key** | **string**|  | [optional] |
| **authorization** | **string**|  | [optional] |

### Return type

**mixed**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `rotateSecretWebhooksV1WebhooksEndpointsRotatePost()`

```php
rotateSecretWebhooksV1WebhooksEndpointsRotatePost($rotate_secret, $x_api_key, $authorization): mixed
```

Rotate Secret

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\WebhooksApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$rotate_secret = new \MailSafePro\Model\RotateSecret(); // \MailSafePro\Model\RotateSecret
$x_api_key = 'x_api_key_example'; // string
$authorization = 'authorization_example'; // string

try {
    $result = $apiInstance->rotateSecretWebhooksV1WebhooksEndpointsRotatePost($rotate_secret, $x_api_key, $authorization);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling WebhooksApi->rotateSecretWebhooksV1WebhooksEndpointsRotatePost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **rotate_secret** | [**\MailSafePro\Model\RotateSecret**](../Model/RotateSecret.md)|  | |
| **x_api_key** | **string**|  | [optional] |
| **authorization** | **string**|  | [optional] |

### Return type

**mixed**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `rotateSecretWebhooksV1WebhooksEndpointsRotatePost_0()`

```php
rotateSecretWebhooksV1WebhooksEndpointsRotatePost_0($rotate_secret, $x_api_key, $authorization): mixed
```

Rotate Secret

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\WebhooksApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$rotate_secret = new \MailSafePro\Model\RotateSecret(); // \MailSafePro\Model\RotateSecret
$x_api_key = 'x_api_key_example'; // string
$authorization = 'authorization_example'; // string

try {
    $result = $apiInstance->rotateSecretWebhooksV1WebhooksEndpointsRotatePost_0($rotate_secret, $x_api_key, $authorization);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling WebhooksApi->rotateSecretWebhooksV1WebhooksEndpointsRotatePost_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **rotate_secret** | [**\MailSafePro\Model\RotateSecret**](../Model/RotateSecret.md)|  | |
| **x_api_key** | **string**|  | [optional] |
| **authorization** | **string**|  | [optional] |

### Return type

**mixed**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
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


$apiInstance = new MailSafePro\Api\WebhooksApi(
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
    echo 'Exception when calling WebhooksApi->testWebhookWebhooksManagementWebhooksWebhookIdTestPost: ', $e->getMessage(), PHP_EOL;
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


$apiInstance = new MailSafePro\Api\WebhooksApi(
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
    echo 'Exception when calling WebhooksApi->updateWebhookWebhooksManagementWebhooksWebhookIdPatch: ', $e->getMessage(), PHP_EOL;
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
