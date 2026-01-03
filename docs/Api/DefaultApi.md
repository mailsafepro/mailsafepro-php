# MailSafePro\DefaultApi



All URIs are relative to http://localhost, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**askGeminiGeminiGet()**](DefaultApi.md#askGeminiGeminiGet) | **GET** /gemini | Ask Gemini |
| [**runAuditAdminAuditProjectPost()**](DefaultApi.md#runAuditAdminAuditProjectPost) | **POST** /admin/audit_project | Run Audit |


## `askGeminiGeminiGet()`

```php
askGeminiGeminiGet($prompt): mixed
```

Ask Gemini

Llama a Gemini para generar texto a partir de un prompt

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$prompt = 'prompt_example'; // string

try {
    $result = $apiInstance->askGeminiGeminiGet($prompt);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->askGeminiGeminiGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **prompt** | **string**|  | |

### Return type

**mixed**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `runAuditAdminAuditProjectPost()`

```php
runAuditAdminAuditProjectPost($path, $x_audit_token): mixed
```

Run Audit

Lanza auditoría en path (ruta absoluta o relativa a la raíz del proyecto). Header obligatorio: X-Audit-Token: <AUDIT_SECRET>

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$path = '.'; // string
$x_audit_token = 'x_audit_token_example'; // string

try {
    $result = $apiInstance->runAuditAdminAuditProjectPost($path, $x_audit_token);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->runAuditAdminAuditProjectPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **path** | **string**|  | [optional] [default to &#39;.&#39;] |
| **x_audit_token** | **string**|  | [optional] |

### Return type

**mixed**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
