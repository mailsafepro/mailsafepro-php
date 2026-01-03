# MailSafePro\AuthenticationApi



All URIs are relative to http://localhost, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**authHealthCheckAuthHealthAuthGet()**](AuthenticationApi.md#authHealthCheckAuthHealthAuthGet) | **GET** /auth/health/auth | Auth Health Check |
| [**authHealthCheckAuthHealthAuthGet_0()**](AuthenticationApi.md#authHealthCheckAuthHealthAuthGet_0) | **GET** /auth/health/auth | Auth Health Check |
| [**authHealthCheckAuthHealthAuthHead()**](AuthenticationApi.md#authHealthCheckAuthHealthAuthHead) | **HEAD** /auth/health/auth | Auth Health Check |
| [**authHealthCheckAuthHealthAuthHead_0()**](AuthenticationApi.md#authHealthCheckAuthHealthAuthHead_0) | **HEAD** /auth/health/auth | Auth Health Check |
| [**deleteAccountAuthDeleteDelete()**](AuthenticationApi.md#deleteAccountAuthDeleteDelete) | **DELETE** /auth/delete | Delete Account |
| [**deleteAccountAuthDeleteDelete_0()**](AuthenticationApi.md#deleteAccountAuthDeleteDelete_0) | **DELETE** /auth/delete | Delete Account |
| [**getCurrentUserAuthMeGet()**](AuthenticationApi.md#getCurrentUserAuthMeGet) | **GET** /auth/me | Get Current User |
| [**getCurrentUserAuthMeGet_0()**](AuthenticationApi.md#getCurrentUserAuthMeGet_0) | **GET** /auth/me | Get Current User |
| [**loginWebUserAuthLoginPost()**](AuthenticationApi.md#loginWebUserAuthLoginPost) | **POST** /auth/login | Login Web User |
| [**loginWebUserAuthLoginPost_0()**](AuthenticationApi.md#loginWebUserAuthLoginPost_0) | **POST** /auth/login | Login Web User |
| [**logoutAuthLogoutPost()**](AuthenticationApi.md#logoutAuthLogoutPost) | **POST** /auth/logout | Logout |
| [**logoutAuthLogoutPost_0()**](AuthenticationApi.md#logoutAuthLogoutPost_0) | **POST** /auth/logout | Logout |
| [**refreshTokenAuthRefreshPost()**](AuthenticationApi.md#refreshTokenAuthRefreshPost) | **POST** /auth/refresh | Refresh Token |
| [**refreshTokenAuthRefreshPost_0()**](AuthenticationApi.md#refreshTokenAuthRefreshPost_0) | **POST** /auth/refresh | Refresh Token |
| [**registerWebUserAuthRegisterPost()**](AuthenticationApi.md#registerWebUserAuthRegisterPost) | **POST** /auth/register | Register Web User |
| [**registerWebUserAuthRegisterPost_0()**](AuthenticationApi.md#registerWebUserAuthRegisterPost_0) | **POST** /auth/register | Register Web User |
| [**rotateApiKeyAuthRotateKeyPost()**](AuthenticationApi.md#rotateApiKeyAuthRotateKeyPost) | **POST** /auth/rotate-key | Rotate Api Key |
| [**rotateApiKeyAuthRotateKeyPost_0()**](AuthenticationApi.md#rotateApiKeyAuthRotateKeyPost_0) | **POST** /auth/rotate-key | Rotate Api Key |


## `authHealthCheckAuthHealthAuthGet()`

```php
authHealthCheckAuthHealthAuthGet(): mixed
```

Auth Health Check

Health check para autenticación: Redis, JWT y hashing.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\AuthenticationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->authHealthCheckAuthHealthAuthGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthenticationApi->authHealthCheckAuthHealthAuthGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

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

## `authHealthCheckAuthHealthAuthGet_0()`

```php
authHealthCheckAuthHealthAuthGet_0(): mixed
```

Auth Health Check

Health check para autenticación: Redis, JWT y hashing.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\AuthenticationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->authHealthCheckAuthHealthAuthGet_0();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthenticationApi->authHealthCheckAuthHealthAuthGet_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

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

## `authHealthCheckAuthHealthAuthHead()`

```php
authHealthCheckAuthHealthAuthHead(): mixed
```

Auth Health Check

Health check para autenticación: Redis, JWT y hashing.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\AuthenticationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->authHealthCheckAuthHealthAuthHead();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthenticationApi->authHealthCheckAuthHealthAuthHead: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

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

## `authHealthCheckAuthHealthAuthHead_0()`

```php
authHealthCheckAuthHealthAuthHead_0(): mixed
```

Auth Health Check

Health check para autenticación: Redis, JWT y hashing.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\AuthenticationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->authHealthCheckAuthHealthAuthHead_0();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthenticationApi->authHealthCheckAuthHealthAuthHead_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

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

## `deleteAccountAuthDeleteDelete()`

```php
deleteAccountAuthDeleteDelete(): mixed
```

Delete Account

Elimina la cuenta del usuario autenticado y todos sus datos relacionados.  ⚠️ ADVERTENCIA: Esta operación es IRREVERSIBLE.  Elimina: - Datos del usuario - Todas las API keys - Usage/quota - Suscripciones - Rate limits - Tokens relacionados  Security: - Solo el usuario puede eliminarse a sí mismo (o admin) - Requiere autenticación válida - Registra la acción en logs para auditoría - Rate limited para prevenir abuse

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\AuthenticationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->deleteAccountAuthDeleteDelete();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthenticationApi->deleteAccountAuthDeleteDelete: ', $e->getMessage(), PHP_EOL;
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

## `deleteAccountAuthDeleteDelete_0()`

```php
deleteAccountAuthDeleteDelete_0(): mixed
```

Delete Account

Elimina la cuenta del usuario autenticado y todos sus datos relacionados.  ⚠️ ADVERTENCIA: Esta operación es IRREVERSIBLE.  Elimina: - Datos del usuario - Todas las API keys - Usage/quota - Suscripciones - Rate limits - Tokens relacionados  Security: - Solo el usuario puede eliminarse a sí mismo (o admin) - Requiere autenticación válida - Registra la acción en logs para auditoría - Rate limited para prevenir abuse

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\AuthenticationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->deleteAccountAuthDeleteDelete_0();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthenticationApi->deleteAccountAuthDeleteDelete_0: ', $e->getMessage(), PHP_EOL;
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

## `getCurrentUserAuthMeGet()`

```php
getCurrentUserAuthMeGet(): object
```

Get Current User

Devuelve información básica del usuario actual.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\AuthenticationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->getCurrentUserAuthMeGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthenticationApi->getCurrentUserAuthMeGet: ', $e->getMessage(), PHP_EOL;
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

## `getCurrentUserAuthMeGet_0()`

```php
getCurrentUserAuthMeGet_0(): object
```

Get Current User

Devuelve información básica del usuario actual.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\AuthenticationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->getCurrentUserAuthMeGet_0();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthenticationApi->getCurrentUserAuthMeGet_0: ', $e->getMessage(), PHP_EOL;
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

## `loginWebUserAuthLoginPost()`

```php
loginWebUserAuthLoginPost($user_login): object
```

Login Web User

Login de usuario para panel web.  Security features: - Rate limiting por email + IP - Timing attack protection - Generic error messages - PII masking en logs

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\AuthenticationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_login = new \MailSafePro\Model\UserLogin(); // \MailSafePro\Model\UserLogin

try {
    $result = $apiInstance->loginWebUserAuthLoginPost($user_login);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthenticationApi->loginWebUserAuthLoginPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **user_login** | [**\MailSafePro\Model\UserLogin**](../Model/UserLogin.md)|  | |

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `loginWebUserAuthLoginPost_0()`

```php
loginWebUserAuthLoginPost_0($user_login): object
```

Login Web User

Login de usuario para panel web.  Security features: - Rate limiting por email + IP - Timing attack protection - Generic error messages - PII masking en logs

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\AuthenticationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_login = new \MailSafePro\Model\UserLogin(); // \MailSafePro\Model\UserLogin

try {
    $result = $apiInstance->loginWebUserAuthLoginPost_0($user_login);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthenticationApi->loginWebUserAuthLoginPost_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **user_login** | [**\MailSafePro\Model\UserLogin**](../Model/UserLogin.md)|  | |

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `logoutAuthLogoutPost()`

```php
logoutAuthLogoutPost(): mixed
```

Logout

Logout idempotente: - Si el access token es válido, lo añade a la blacklist. - Si el access token está expirado, responde 200 indicando que ya estaba expirado. - Solo devuelve 401 si el token es completamente inválido (firma/claims corruptos). - Intenta revocar el refresh token si se proporciona.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\AuthenticationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->logoutAuthLogoutPost();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthenticationApi->logoutAuthLogoutPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

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

## `logoutAuthLogoutPost_0()`

```php
logoutAuthLogoutPost_0(): mixed
```

Logout

Logout idempotente: - Si el access token es válido, lo añade a la blacklist. - Si el access token está expirado, responde 200 indicando que ya estaba expirado. - Solo devuelve 401 si el token es completamente inválido (firma/claims corruptos). - Intenta revocar el refresh token si se proporciona.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\AuthenticationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->logoutAuthLogoutPost_0();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthenticationApi->logoutAuthLogoutPost_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

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

## `refreshTokenAuthRefreshPost()`

```php
refreshTokenAuthRefreshPost(): object
```

Refresh Token

Crea un nuevo par de tokens a partir de un refresh token válido y no revocado.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\AuthenticationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->refreshTokenAuthRefreshPost();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthenticationApi->refreshTokenAuthRefreshPost: ', $e->getMessage(), PHP_EOL;
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

## `refreshTokenAuthRefreshPost_0()`

```php
refreshTokenAuthRefreshPost_0(): object
```

Refresh Token

Crea un nuevo par de tokens a partir de un refresh token válido y no revocado.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\AuthenticationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->refreshTokenAuthRefreshPost_0();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthenticationApi->refreshTokenAuthRefreshPost_0: ', $e->getMessage(), PHP_EOL;
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

## `registerWebUserAuthRegisterPost()`

```php
registerWebUserAuthRegisterPost($user_register): object
```

Register Web User

Registro de usuario para panel web: crea usuario, API key y tokens.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\AuthenticationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_register = new \MailSafePro\Model\UserRegister(); // \MailSafePro\Model\UserRegister

try {
    $result = $apiInstance->registerWebUserAuthRegisterPost($user_register);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthenticationApi->registerWebUserAuthRegisterPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **user_register** | [**\MailSafePro\Model\UserRegister**](../Model/UserRegister.md)|  | |

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `registerWebUserAuthRegisterPost_0()`

```php
registerWebUserAuthRegisterPost_0($user_register): object
```

Register Web User

Registro de usuario para panel web: crea usuario, API key y tokens.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\AuthenticationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_register = new \MailSafePro\Model\UserRegister(); // \MailSafePro\Model\UserRegister

try {
    $result = $apiInstance->registerWebUserAuthRegisterPost_0($user_register);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthenticationApi->registerWebUserAuthRegisterPost_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **user_register** | [**\MailSafePro\Model\UserRegister**](../Model/UserRegister.md)|  | |

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `rotateApiKeyAuthRotateKeyPost()`

```php
rotateApiKeyAuthRotateKeyPost($key_rotation_request): object
```

Rotate Api Key

Rotación de API keys con período de gracia; acceso restringido a admin.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\AuthenticationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$key_rotation_request = new \MailSafePro\Model\KeyRotationRequest(); // \MailSafePro\Model\KeyRotationRequest

try {
    $result = $apiInstance->rotateApiKeyAuthRotateKeyPost($key_rotation_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthenticationApi->rotateApiKeyAuthRotateKeyPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key_rotation_request** | [**\MailSafePro\Model\KeyRotationRequest**](../Model/KeyRotationRequest.md)|  | |

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

## `rotateApiKeyAuthRotateKeyPost_0()`

```php
rotateApiKeyAuthRotateKeyPost_0($key_rotation_request): object
```

Rotate Api Key

Rotación de API keys con período de gracia; acceso restringido a admin.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\AuthenticationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$key_rotation_request = new \MailSafePro\Model\KeyRotationRequest(); // \MailSafePro\Model\KeyRotationRequest

try {
    $result = $apiInstance->rotateApiKeyAuthRotateKeyPost_0($key_rotation_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthenticationApi->rotateApiKeyAuthRotateKeyPost_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key_rotation_request** | [**\MailSafePro\Model\KeyRotationRequest**](../Model/KeyRotationRequest.md)|  | |

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
