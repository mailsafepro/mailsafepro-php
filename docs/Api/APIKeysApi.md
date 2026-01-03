# MailSafePro\APIKeysApi



All URIs are relative to http://localhost, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createApiKeyApiKeysPost()**](APIKeysApi.md#createApiKeyApiKeysPost) | **POST** /api-keys | Create Api Key |
| [**createApiKeyApiKeysPost_0()**](APIKeysApi.md#createApiKeyApiKeysPost_0) | **POST** /api-keys | Create Api Key |
| [**forceSyncApiKeysForceSyncPost()**](APIKeysApi.md#forceSyncApiKeysForceSyncPost) | **POST** /api-keys/force-sync | Force Sync |
| [**forceSyncApiKeysForceSyncPost_0()**](APIKeysApi.md#forceSyncApiKeysForceSyncPost_0) | **POST** /api-keys/force-sync | Force Sync |
| [**getApiKeyValueApiKeysKeyHashValueGet()**](APIKeysApi.md#getApiKeyValueApiKeysKeyHashValueGet) | **GET** /api-keys/{key_hash}/value | Get Api Key Value |
| [**getApiKeyValueApiKeysKeyHashValueGet_0()**](APIKeysApi.md#getApiKeyValueApiKeysKeyHashValueGet_0) | **GET** /api-keys/{key_hash}/value | Get Api Key Value |
| [**getUsageApiKeysUsageGet()**](APIKeysApi.md#getUsageApiKeysUsageGet) | **GET** /api-keys/usage | Get Usage |
| [**getUsageApiKeysUsageGet_0()**](APIKeysApi.md#getUsageApiKeysUsageGet_0) | **GET** /api-keys/usage | Get Usage |
| [**listApiKeysApiKeysGet()**](APIKeysApi.md#listApiKeysApiKeysGet) | **GET** /api-keys | List Api Keys |
| [**listApiKeysApiKeysGet_0()**](APIKeysApi.md#listApiKeysApiKeysGet_0) | **GET** /api-keys | List Api Keys |
| [**repairUserDataEndpointApiKeysRepairDataPost()**](APIKeysApi.md#repairUserDataEndpointApiKeysRepairDataPost) | **POST** /api-keys/repair-data | Repair User Data Endpoint |
| [**repairUserDataEndpointApiKeysRepairDataPost_0()**](APIKeysApi.md#repairUserDataEndpointApiKeysRepairDataPost_0) | **POST** /api-keys/repair-data | Repair User Data Endpoint |
| [**revokeApiKeyApiKeysKeyHashRevokeDelete()**](APIKeysApi.md#revokeApiKeyApiKeysKeyHashRevokeDelete) | **DELETE** /api-keys/{key_hash}/revoke | Revoke Api Key |
| [**revokeApiKeyApiKeysKeyHashRevokeDelete_0()**](APIKeysApi.md#revokeApiKeyApiKeysKeyHashRevokeDelete_0) | **DELETE** /api-keys/{key_hash}/revoke | Revoke Api Key |
| [**rotateApiKeyApiKeysKeyHashRotatePost()**](APIKeysApi.md#rotateApiKeyApiKeysKeyHashRotatePost) | **POST** /api-keys/{key_hash}/rotate | Rotate Api Key |
| [**rotateApiKeyApiKeysKeyHashRotatePost_0()**](APIKeysApi.md#rotateApiKeyApiKeysKeyHashRotatePost_0) | **POST** /api-keys/{key_hash}/rotate | Rotate Api Key |
| [**syncPlanKeysApiKeysSyncPlanKeysPost()**](APIKeysApi.md#syncPlanKeysApiKeysSyncPlanKeysPost) | **POST** /api-keys/sync-plan-keys | Sync Plan Keys |
| [**syncPlanKeysApiKeysSyncPlanKeysPost_0()**](APIKeysApi.md#syncPlanKeysApiKeysSyncPlanKeysPost_0) | **POST** /api-keys/sync-plan-keys | Sync Plan Keys |


## `createApiKeyApiKeysPost()`

```php
createApiKeyApiKeysPost($api_key_create_request): object
```

Create Api Key

Create a new API key with atomic transaction. Generates cryptographically secure API keys with proper scoping based on user's current plan. Enforces maximum key limits.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\APIKeysApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$api_key_create_request = new \MailSafePro\Model\APIKeyCreateRequest(); // \MailSafePro\Model\APIKeyCreateRequest

try {
    $result = $apiInstance->createApiKeyApiKeysPost($api_key_create_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling APIKeysApi->createApiKeyApiKeysPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **api_key_create_request** | [**\MailSafePro\Model\APIKeyCreateRequest**](../Model/APIKeyCreateRequest.md)|  | |

### Return type

**object**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createApiKeyApiKeysPost_0()`

```php
createApiKeyApiKeysPost_0($api_key_create_request): object
```

Create Api Key

Create a new API key with atomic transaction. Generates cryptographically secure API keys with proper scoping based on user's current plan. Enforces maximum key limits.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\APIKeysApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$api_key_create_request = new \MailSafePro\Model\APIKeyCreateRequest(); // \MailSafePro\Model\APIKeyCreateRequest

try {
    $result = $apiInstance->createApiKeyApiKeysPost_0($api_key_create_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling APIKeysApi->createApiKeyApiKeysPost_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **api_key_create_request** | [**\MailSafePro\Model\APIKeyCreateRequest**](../Model/APIKeyCreateRequest.md)|  | |

### Return type

**object**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `forceSyncApiKeysForceSyncPost()`

```php
forceSyncApiKeysForceSyncPost(): object
```

Force Sync

Force synchronization of user data with rate limiting. Synchronizes API keys with current plan and clears relevant caches. Limited to one sync per 5 minutes per user.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\APIKeysApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->forceSyncApiKeysForceSyncPost();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling APIKeysApi->forceSyncApiKeysForceSyncPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `forceSyncApiKeysForceSyncPost_0()`

```php
forceSyncApiKeysForceSyncPost_0(): object
```

Force Sync

Force synchronization of user data with rate limiting. Synchronizes API keys with current plan and clears relevant caches. Limited to one sync per 5 minutes per user.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\APIKeysApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->forceSyncApiKeysForceSyncPost_0();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling APIKeysApi->forceSyncApiKeysForceSyncPost_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getApiKeyValueApiKeysKeyHashValueGet()`

```php
getApiKeyValueApiKeysKeyHashValueGet($key_hash): object
```

Get Api Key Value

Retrieve API key metadata (security-safe). Returns key information without exposing the actual key value. Used for key management and verification purposes.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\APIKeysApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$key_hash = 'key_hash_example'; // string

try {
    $result = $apiInstance->getApiKeyValueApiKeysKeyHashValueGet($key_hash);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling APIKeysApi->getApiKeyValueApiKeysKeyHashValueGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key_hash** | **string**|  | |

### Return type

**object**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getApiKeyValueApiKeysKeyHashValueGet_0()`

```php
getApiKeyValueApiKeysKeyHashValueGet_0($key_hash): object
```

Get Api Key Value

Retrieve API key metadata (security-safe). Returns key information without exposing the actual key value. Used for key management and verification purposes.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\APIKeysApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$key_hash = 'key_hash_example'; // string

try {
    $result = $apiInstance->getApiKeyValueApiKeysKeyHashValueGet_0($key_hash);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling APIKeysApi->getApiKeyValueApiKeysKeyHashValueGet_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key_hash** | **string**|  | |

### Return type

**object**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getUsageApiKeysUsageGet()`

```php
getUsageApiKeysUsageGet($x_api_key, $authorization): object
```

Get Usage

Get current API usage statistics. Returns usage count, limits, and remaining requests for today. Works with both API keys and JWT tokens.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\APIKeysApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$x_api_key = 'x_api_key_example'; // string
$authorization = 'authorization_example'; // string

try {
    $result = $apiInstance->getUsageApiKeysUsageGet($x_api_key, $authorization);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling APIKeysApi->getUsageApiKeysUsageGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **x_api_key** | **string**|  | [optional] |
| **authorization** | **string**|  | [optional] |

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getUsageApiKeysUsageGet_0()`

```php
getUsageApiKeysUsageGet_0($x_api_key, $authorization): object
```

Get Usage

Get current API usage statistics. Returns usage count, limits, and remaining requests for today. Works with both API keys and JWT tokens.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\APIKeysApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$x_api_key = 'x_api_key_example'; // string
$authorization = 'authorization_example'; // string

try {
    $result = $apiInstance->getUsageApiKeysUsageGet_0($x_api_key, $authorization);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling APIKeysApi->getUsageApiKeysUsageGet_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **x_api_key** | **string**|  | [optional] |
| **authorization** | **string**|  | [optional] |

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listApiKeysApiKeysGet()`

```php
listApiKeysApiKeysGet(): \MailSafePro\Model\APIKeyListResponse
```

List Api Keys

List all API keys for current user with consistent IDs. Returns comprehensive key metadata including status, scopes, and usage information. Handles corrupted key data gracefully.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\APIKeysApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->listApiKeysApiKeysGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling APIKeysApi->listApiKeysApiKeysGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\MailSafePro\Model\APIKeyListResponse**](../Model/APIKeyListResponse.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listApiKeysApiKeysGet_0()`

```php
listApiKeysApiKeysGet_0(): \MailSafePro\Model\APIKeyListResponse
```

List Api Keys

List all API keys for current user with consistent IDs. Returns comprehensive key metadata including status, scopes, and usage information. Handles corrupted key data gracefully.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\APIKeysApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->listApiKeysApiKeysGet_0();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling APIKeysApi->listApiKeysApiKeysGet_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\MailSafePro\Model\APIKeyListResponse**](../Model/APIKeyListResponse.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `repairUserDataEndpointApiKeysRepairDataPost()`

```php
repairUserDataEndpointApiKeysRepairDataPost(): array<string,string>
```

Repair User Data Endpoint

Emergency data repair endpoint - ADMINISTRATORS ONLY WARNING: Critical operation; relies on admin scope verification at runtime.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\APIKeysApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->repairUserDataEndpointApiKeysRepairDataPost();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling APIKeysApi->repairUserDataEndpointApiKeysRepairDataPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

**array<string,string>**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `repairUserDataEndpointApiKeysRepairDataPost_0()`

```php
repairUserDataEndpointApiKeysRepairDataPost_0(): array<string,string>
```

Repair User Data Endpoint

Emergency data repair endpoint - ADMINISTRATORS ONLY WARNING: Critical operation; relies on admin scope verification at runtime.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\APIKeysApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->repairUserDataEndpointApiKeysRepairDataPost_0();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling APIKeysApi->repairUserDataEndpointApiKeysRepairDataPost_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

**array<string,string>**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `revokeApiKeyApiKeysKeyHashRevokeDelete()`

```php
revokeApiKeyApiKeysKeyHashRevokeDelete($key_hash): mixed
```

Revoke Api Key

Revoke an API key with atomic transaction. Immediately invalidates the key and removes it from active sets. Provides audit trail for security compliance.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\APIKeysApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$key_hash = 'key_hash_example'; // string

try {
    $result = $apiInstance->revokeApiKeyApiKeysKeyHashRevokeDelete($key_hash);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling APIKeysApi->revokeApiKeyApiKeysKeyHashRevokeDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key_hash** | **string**|  | |

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

## `revokeApiKeyApiKeysKeyHashRevokeDelete_0()`

```php
revokeApiKeyApiKeysKeyHashRevokeDelete_0($key_hash): mixed
```

Revoke Api Key

Revoke an API key with atomic transaction. Immediately invalidates the key and removes it from active sets. Provides audit trail for security compliance.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\APIKeysApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$key_hash = 'key_hash_example'; // string

try {
    $result = $apiInstance->revokeApiKeyApiKeysKeyHashRevokeDelete_0($key_hash);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling APIKeysApi->revokeApiKeyApiKeysKeyHashRevokeDelete_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key_hash** | **string**|  | |

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

## `rotateApiKeyApiKeysKeyHashRotatePost()`

```php
rotateApiKeyApiKeysKeyHashRotatePost($key_hash): object
```

Rotate Api Key

Rotate API key with grace period. Generates a new key while keeping the old one active for 7 days to allow for smooth transition in client applications.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\APIKeysApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$key_hash = 'key_hash_example'; // string

try {
    $result = $apiInstance->rotateApiKeyApiKeysKeyHashRotatePost($key_hash);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling APIKeysApi->rotateApiKeyApiKeysKeyHashRotatePost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key_hash** | **string**|  | |

### Return type

**object**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `rotateApiKeyApiKeysKeyHashRotatePost_0()`

```php
rotateApiKeyApiKeysKeyHashRotatePost_0($key_hash): object
```

Rotate Api Key

Rotate API key with grace period. Generates a new key while keeping the old one active for 7 days to allow for smooth transition in client applications.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\APIKeysApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$key_hash = 'key_hash_example'; // string

try {
    $result = $apiInstance->rotateApiKeyApiKeysKeyHashRotatePost_0($key_hash);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling APIKeysApi->rotateApiKeyApiKeysKeyHashRotatePost_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key_hash** | **string**|  | |

### Return type

**object**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `syncPlanKeysApiKeysSyncPlanKeysPost()`

```php
syncPlanKeysApiKeysSyncPlanKeysPost(): object
```

Sync Plan Keys

Synchronize current plan with all user API keys. Ensures all existing keys have the correct scopes and permissions based on the user's current subscription plan.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\APIKeysApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->syncPlanKeysApiKeysSyncPlanKeysPost();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling APIKeysApi->syncPlanKeysApiKeysSyncPlanKeysPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `syncPlanKeysApiKeysSyncPlanKeysPost_0()`

```php
syncPlanKeysApiKeysSyncPlanKeysPost_0(): object
```

Sync Plan Keys

Synchronize current plan with all user API keys. Ensures all existing keys have the correct scopes and permissions based on the user's current subscription plan.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\APIKeysApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->syncPlanKeysApiKeysSyncPlanKeysPost_0();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling APIKeysApi->syncPlanKeysApiKeysSyncPlanKeysPost_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
