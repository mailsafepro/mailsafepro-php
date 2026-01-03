# MailSafePro\ValidationApi



All URIs are relative to http://localhost, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**batchValidateEmailsValidateBatchPost()**](ValidationApi.md#batchValidateEmailsValidateBatchPost) | **POST** /validate/batch | Batch Email Validation |
| [**batchValidateUploadValidateBatchUploadPost()**](ValidationApi.md#batchValidateUploadValidateBatchUploadPost) | **POST** /validate/batch/upload | Batch Email Validation via File Upload |
| [**getCacheStatsValidateStatsCacheGet()**](ValidationApi.md#getCacheStatsValidateStatsCacheGet) | **GET** /validate/stats/cache | Get Cache Stats |
| [**getUsageStatsValidateStatsUsageGet()**](ValidationApi.md#getUsageStatsValidateStatsUsageGet) | **GET** /validate/stats/usage | Get Usage Stats |
| [**healthCheckValidateHealthGet()**](ValidationApi.md#healthCheckValidateHealthGet) | **GET** /validate/health | Health Check |
| [**healthCheckValidateHealthHead()**](ValidationApi.md#healthCheckValidateHealthHead) | **HEAD** /validate/health | Health Check |
| [**validateEmailEndpointValidateEmailPost()**](ValidationApi.md#validateEmailEndpointValidateEmailPost) | **POST** /validate/email | Validate Email Endpoint |


## `batchValidateEmailsValidateBatchPost()`

```php
batchValidateEmailsValidateBatchPost($batch_validation_request, $x_api_key, $authorization): \MailSafePro\Model\BatchEmailResponse
```

Batch Email Validation

Valida múltiples direcciones de email en una sola solicitud.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\ValidationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$batch_validation_request = new \MailSafePro\Model\BatchValidationRequest(); // \MailSafePro\Model\BatchValidationRequest
$x_api_key = 'x_api_key_example'; // string
$authorization = 'authorization_example'; // string

try {
    $result = $apiInstance->batchValidateEmailsValidateBatchPost($batch_validation_request, $x_api_key, $authorization);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ValidationApi->batchValidateEmailsValidateBatchPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **batch_validation_request** | [**\MailSafePro\Model\BatchValidationRequest**](../Model/BatchValidationRequest.md)|  | |
| **x_api_key** | **string**|  | [optional] |
| **authorization** | **string**|  | [optional] |

### Return type

[**\MailSafePro\Model\BatchEmailResponse**](../Model/BatchEmailResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `batchValidateUploadValidateBatchUploadPost()`

```php
batchValidateUploadValidateBatchUploadPost($file, $x_api_key, $authorization, $column, $include_raw_dns, $check_smtp): mixed
```

Batch Email Validation via File Upload

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\ValidationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$file = '/path/to/file.txt'; // \SplFileObject
$x_api_key = 'x_api_key_example'; // string
$authorization = 'authorization_example'; // string
$column = 'column_example'; // string
$include_raw_dns = false; // bool
$check_smtp = false; // bool

try {
    $result = $apiInstance->batchValidateUploadValidateBatchUploadPost($file, $x_api_key, $authorization, $column, $include_raw_dns, $check_smtp);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ValidationApi->batchValidateUploadValidateBatchUploadPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **file** | **\SplFileObject****\SplFileObject**|  | |
| **x_api_key** | **string**|  | [optional] |
| **authorization** | **string**|  | [optional] |
| **column** | **string**|  | [optional] |
| **include_raw_dns** | **bool**|  | [optional] [default to false] |
| **check_smtp** | **bool**|  | [optional] [default to false] |

### Return type

**mixed**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getCacheStatsValidateStatsCacheGet()`

```php
getCacheStatsValidateStatsCacheGet(): object
```

Get Cache Stats

Obtiene estadísticas de cache del sistema.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\ValidationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->getCacheStatsValidateStatsCacheGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ValidationApi->getCacheStatsValidateStatsCacheGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

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

## `getUsageStatsValidateStatsUsageGet()`

```php
getUsageStatsValidateStatsUsageGet($x_api_key, $authorization): object
```

Get Usage Stats

Obtiene estadísticas de uso del cliente actual.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\ValidationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$x_api_key = 'x_api_key_example'; // string
$authorization = 'authorization_example'; // string

try {
    $result = $apiInstance->getUsageStatsValidateStatsUsageGet($x_api_key, $authorization);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ValidationApi->getUsageStatsValidateStatsUsageGet: ', $e->getMessage(), PHP_EOL;
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

## `healthCheckValidateHealthGet()`

```php
healthCheckValidateHealthGet(): object
```

Health Check

Health check completo del servicio de validación.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\ValidationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->healthCheckValidateHealthGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ValidationApi->healthCheckValidateHealthGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

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

## `healthCheckValidateHealthHead()`

```php
healthCheckValidateHealthHead(): object
```

Health Check

Health check completo del servicio de validación.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\ValidationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->healthCheckValidateHealthHead();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ValidationApi->healthCheckValidateHealthHead: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

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

## `validateEmailEndpointValidateEmailPost()`

```php
validateEmailEndpointValidateEmailPost($email_validation_request, $x_api_key, $authorization): mixed
```

Validate Email Endpoint

✅ Endpoint de validación de email con timeout y fallback robusto.  Cambios principales: - Timeout explícito por plan (FREE: 15s, PREMIUM: 45s, ENTERPRISE: 60s) - Fallback BASIC seguro si se vence - SIEMPRE retorna JSONResponse válida - client_plan en TODAS las respuestas - spam_trap_check ejecutado ANTES del timeout para estar disponible en fallback - Manejo de errores con ResponseBuilder - ✅ NUEVO: Soporte para TLD .test en testing_mode

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\ValidationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$email_validation_request = new \MailSafePro\Model\EmailValidationRequest(); // \MailSafePro\Model\EmailValidationRequest
$x_api_key = 'x_api_key_example'; // string
$authorization = 'authorization_example'; // string

try {
    $result = $apiInstance->validateEmailEndpointValidateEmailPost($email_validation_request, $x_api_key, $authorization);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ValidationApi->validateEmailEndpointValidateEmailPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **email_validation_request** | [**\MailSafePro\Model\EmailValidationRequest**](../Model/EmailValidationRequest.md)|  | |
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
