# MailSafePro\HealthApi



All URIs are relative to http://localhost, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**basicHealthHealthGet()**](HealthApi.md#basicHealthHealthGet) | **GET** /health | Basic health check |
| [**basicHealthHealthGet_0()**](HealthApi.md#basicHealthHealthGet_0) | **GET** /health | Basic health check |
| [**circuitBreakerStatusAdminCircuitBreakerStatusGet()**](HealthApi.md#circuitBreakerStatusAdminCircuitBreakerStatusGet) | **GET** /admin/circuit-breaker-status | Circuit Breaker Status |
| [**detailedHealthHealthDetailedGet()**](HealthApi.md#detailedHealthHealthDetailedGet) | **GET** /health/detailed | Detailed health check |
| [**detailedHealthHealthDetailedGet_0()**](HealthApi.md#detailedHealthHealthDetailedGet_0) | **GET** /health/detailed | Detailed health check |
| [**healthcheckHealthcheckGet()**](HealthApi.md#healthcheckHealthcheckGet) | **GET** /healthcheck | Healthcheck |
| [**healthcheckHealthcheckHead()**](HealthApi.md#healthcheckHealthcheckHead) | **HEAD** /healthcheck | Healthcheck |
| [**livenessCheckHealthLivenessGet()**](HealthApi.md#livenessCheckHealthLivenessGet) | **GET** /health/liveness | Liveness Check |
| [**livenessHealthLiveGet()**](HealthApi.md#livenessHealthLiveGet) | **GET** /health/live | Liveness probe (Kubernetes) |
| [**livenessHealthLiveGet_0()**](HealthApi.md#livenessHealthLiveGet_0) | **GET** /health/live | Liveness probe (Kubernetes) |
| [**readinessCheckHealthReadinessGet()**](HealthApi.md#readinessCheckHealthReadinessGet) | **GET** /health/readiness | Readiness Check |
| [**readinessHealthReadyGet()**](HealthApi.md#readinessHealthReadyGet) | **GET** /health/ready | Readiness probe (Kubernetes) |
| [**readinessHealthReadyGet_0()**](HealthApi.md#readinessHealthReadyGet_0) | **GET** /health/ready | Readiness probe (Kubernetes) |
| [**serviceStatusStatusGet()**](HealthApi.md#serviceStatusStatusGet) | **GET** /status | Service Status |
| [**startupCheckHealthStartupGet()**](HealthApi.md#startupCheckHealthStartupGet) | **GET** /health/startup | Startup Check |


## `basicHealthHealthGet()`

```php
basicHealthHealthGet(): mixed
```

Basic health check

Basic health check for load balancers.  Returns 200 if service is running. Fast response, no dependency checks.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\HealthApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->basicHealthHealthGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HealthApi->basicHealthHealthGet: ', $e->getMessage(), PHP_EOL;
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

## `basicHealthHealthGet_0()`

```php
basicHealthHealthGet_0(): mixed
```

Basic health check

Basic health check for load balancers.  Returns 200 if service is running. Fast response, no dependency checks.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\HealthApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->basicHealthHealthGet_0();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HealthApi->basicHealthHealthGet_0: ', $e->getMessage(), PHP_EOL;
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

## `circuitBreakerStatusAdminCircuitBreakerStatusGet()`

```php
circuitBreakerStatusAdminCircuitBreakerStatusGet(): mixed
```

Circuit Breaker Status

✅ Circuit breaker status for all services. Shows state of Redis, SMTP, DNS, and other circuit breakers.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\HealthApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->circuitBreakerStatusAdminCircuitBreakerStatusGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HealthApi->circuitBreakerStatusAdminCircuitBreakerStatusGet: ', $e->getMessage(), PHP_EOL;
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

## `detailedHealthHealthDetailedGet()`

```php
detailedHealthHealthDetailedGet(): mixed
```

Detailed health check

Detailed health check with all component statuses.  Returns comprehensive health information for monitoring.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\HealthApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->detailedHealthHealthDetailedGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HealthApi->detailedHealthHealthDetailedGet: ', $e->getMessage(), PHP_EOL;
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

## `detailedHealthHealthDetailedGet_0()`

```php
detailedHealthHealthDetailedGet_0(): mixed
```

Detailed health check

Detailed health check with all component statuses.  Returns comprehensive health information for monitoring.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\HealthApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->detailedHealthHealthDetailedGet_0();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HealthApi->detailedHealthHealthDetailedGet_0: ', $e->getMessage(), PHP_EOL;
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

## `healthcheckHealthcheckGet()`

```php
healthcheckHealthcheckGet(): mixed
```

Healthcheck

Basic health check endpoint (backward compatibility)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\HealthApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->healthcheckHealthcheckGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HealthApi->healthcheckHealthcheckGet: ', $e->getMessage(), PHP_EOL;
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

## `healthcheckHealthcheckHead()`

```php
healthcheckHealthcheckHead(): mixed
```

Healthcheck

Basic health check endpoint (backward compatibility)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\HealthApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->healthcheckHealthcheckHead();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HealthApi->healthcheckHealthcheckHead: ', $e->getMessage(), PHP_EOL;
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

## `livenessCheckHealthLivenessGet()`

```php
livenessCheckHealthLivenessGet(): mixed
```

Liveness Check

✅ MEJORA: Kubernetes liveness probe  Returns 200 if the application is alive (not deadlocked) Used by Kubernetes to restart the pod if unhealthy

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\HealthApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->livenessCheckHealthLivenessGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HealthApi->livenessCheckHealthLivenessGet: ', $e->getMessage(), PHP_EOL;
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

## `livenessHealthLiveGet()`

```php
livenessHealthLiveGet(): mixed
```

Liveness probe (Kubernetes)

Kubernetes liveness probe.  Returns 200 if the application is running. Should restart pod if this fails.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\HealthApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->livenessHealthLiveGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HealthApi->livenessHealthLiveGet: ', $e->getMessage(), PHP_EOL;
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

## `livenessHealthLiveGet_0()`

```php
livenessHealthLiveGet_0(): mixed
```

Liveness probe (Kubernetes)

Kubernetes liveness probe.  Returns 200 if the application is running. Should restart pod if this fails.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\HealthApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->livenessHealthLiveGet_0();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HealthApi->livenessHealthLiveGet_0: ', $e->getMessage(), PHP_EOL;
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

## `readinessCheckHealthReadinessGet()`

```php
readinessCheckHealthReadinessGet(): mixed
```

Readiness Check

✅ MEJORA: Kubernetes readiness probe  Returns 200 if the application is ready to serve traffic Checks all critical dependencies (PostgreSQL, Redis, ARQ)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\HealthApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->readinessCheckHealthReadinessGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HealthApi->readinessCheckHealthReadinessGet: ', $e->getMessage(), PHP_EOL;
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

## `readinessHealthReadyGet()`

```php
readinessHealthReadyGet(): mixed
```

Readiness probe (Kubernetes)

Kubernetes readiness probe.  Returns 200 if service is ready to accept traffic. Checks critical dependencies (Redis).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\HealthApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->readinessHealthReadyGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HealthApi->readinessHealthReadyGet: ', $e->getMessage(), PHP_EOL;
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

## `readinessHealthReadyGet_0()`

```php
readinessHealthReadyGet_0(): mixed
```

Readiness probe (Kubernetes)

Kubernetes readiness probe.  Returns 200 if service is ready to accept traffic. Checks critical dependencies (Redis).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\HealthApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->readinessHealthReadyGet_0();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HealthApi->readinessHealthReadyGet_0: ', $e->getMessage(), PHP_EOL;
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

## `serviceStatusStatusGet()`

```php
serviceStatusStatusGet(): mixed
```

Service Status

✅ MEJORA: Detailed service status with feature flags  Shows which features are available and which are running in degraded mode

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\HealthApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->serviceStatusStatusGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HealthApi->serviceStatusStatusGet: ', $e->getMessage(), PHP_EOL;
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

## `startupCheckHealthStartupGet()`

```php
startupCheckHealthStartupGet(): mixed
```

Startup Check

✅ MEJORA: Kubernetes startup probe  Returns 200 once the application has completed startup Used to delay readiness checks until startup is complete

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\HealthApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->startupCheckHealthStartupGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HealthApi->startupCheckHealthStartupGet: ', $e->getMessage(), PHP_EOL;
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
