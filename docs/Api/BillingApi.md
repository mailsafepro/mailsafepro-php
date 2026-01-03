# MailSafePro\BillingApi



All URIs are relative to http://localhost, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**changePlanBillingBillingChangePlanPost()**](BillingApi.md#changePlanBillingBillingChangePlanPost) | **POST** /billing/billing/change-plan | Change Plan |
| [**changePlanBillingBillingChangePlanPost_0()**](BillingApi.md#changePlanBillingBillingChangePlanPost_0) | **POST** /billing/billing/change-plan | Change Plan |
| [**createCheckoutSessionBillingBillingCreateCheckoutSessionPost()**](BillingApi.md#createCheckoutSessionBillingBillingCreateCheckoutSessionPost) | **POST** /billing/billing/create-checkout-session | Create Checkout Session |
| [**createCheckoutSessionBillingBillingCreateCheckoutSessionPost_0()**](BillingApi.md#createCheckoutSessionBillingBillingCreateCheckoutSessionPost_0) | **POST** /billing/billing/create-checkout-session | Create Checkout Session |
| [**getSubscriptionBillingBillingSubscriptionGet()**](BillingApi.md#getSubscriptionBillingBillingSubscriptionGet) | **GET** /billing/billing/subscription | Get Subscription |
| [**getSubscriptionBillingBillingSubscriptionGet_0()**](BillingApi.md#getSubscriptionBillingBillingSubscriptionGet_0) | **GET** /billing/billing/subscription | Get Subscription |
| [**stripeWebhookBillingBillingWebhookPost()**](BillingApi.md#stripeWebhookBillingBillingWebhookPost) | **POST** /billing/billing/webhook | Stripe Webhook |
| [**stripeWebhookBillingBillingWebhookPost_0()**](BillingApi.md#stripeWebhookBillingBillingWebhookPost_0) | **POST** /billing/billing/webhook | Stripe Webhook |
| [**testNotificationBillingBillingTestNotificationPost()**](BillingApi.md#testNotificationBillingBillingTestNotificationPost) | **POST** /billing/billing/test-notification | Test Notification |
| [**testNotificationBillingBillingTestNotificationPost_0()**](BillingApi.md#testNotificationBillingBillingTestNotificationPost_0) | **POST** /billing/billing/test-notification | Test Notification |


## `changePlanBillingBillingChangePlanPost()`

```php
changePlanBillingBillingChangePlanPost($body_change_plan_billing_billing_change_plan_post): object
```

Change Plan

Cambiar el plan del usuario.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\BillingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body_change_plan_billing_billing_change_plan_post = new \MailSafePro\Model\BodyChangePlanBillingBillingChangePlanPost(); // \MailSafePro\Model\BodyChangePlanBillingBillingChangePlanPost

try {
    $result = $apiInstance->changePlanBillingBillingChangePlanPost($body_change_plan_billing_billing_change_plan_post);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BillingApi->changePlanBillingBillingChangePlanPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body_change_plan_billing_billing_change_plan_post** | [**\MailSafePro\Model\BodyChangePlanBillingBillingChangePlanPost**](../Model/BodyChangePlanBillingBillingChangePlanPost.md)|  | |

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

## `changePlanBillingBillingChangePlanPost_0()`

```php
changePlanBillingBillingChangePlanPost_0($body_change_plan_billing_billing_change_plan_post): object
```

Change Plan

Cambiar el plan del usuario.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\BillingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body_change_plan_billing_billing_change_plan_post = new \MailSafePro\Model\BodyChangePlanBillingBillingChangePlanPost(); // \MailSafePro\Model\BodyChangePlanBillingBillingChangePlanPost

try {
    $result = $apiInstance->changePlanBillingBillingChangePlanPost_0($body_change_plan_billing_billing_change_plan_post);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BillingApi->changePlanBillingBillingChangePlanPost_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body_change_plan_billing_billing_change_plan_post** | [**\MailSafePro\Model\BodyChangePlanBillingBillingChangePlanPost**](../Model/BodyChangePlanBillingBillingChangePlanPost.md)|  | |

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

## `createCheckoutSessionBillingBillingCreateCheckoutSessionPost()`

```php
createCheckoutSessionBillingBillingCreateCheckoutSessionPost($checkout_request): \MailSafePro\Model\CheckoutSessionResponse
```

Create Checkout Session

Crea una checkout session de Stripe para suscripción.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\BillingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$checkout_request = new \MailSafePro\Model\CheckoutRequest(); // \MailSafePro\Model\CheckoutRequest

try {
    $result = $apiInstance->createCheckoutSessionBillingBillingCreateCheckoutSessionPost($checkout_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BillingApi->createCheckoutSessionBillingBillingCreateCheckoutSessionPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **checkout_request** | [**\MailSafePro\Model\CheckoutRequest**](../Model/CheckoutRequest.md)|  | |

### Return type

[**\MailSafePro\Model\CheckoutSessionResponse**](../Model/CheckoutSessionResponse.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createCheckoutSessionBillingBillingCreateCheckoutSessionPost_0()`

```php
createCheckoutSessionBillingBillingCreateCheckoutSessionPost_0($checkout_request): \MailSafePro\Model\CheckoutSessionResponse
```

Create Checkout Session

Crea una checkout session de Stripe para suscripción.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\BillingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$checkout_request = new \MailSafePro\Model\CheckoutRequest(); // \MailSafePro\Model\CheckoutRequest

try {
    $result = $apiInstance->createCheckoutSessionBillingBillingCreateCheckoutSessionPost_0($checkout_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BillingApi->createCheckoutSessionBillingBillingCreateCheckoutSessionPost_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **checkout_request** | [**\MailSafePro\Model\CheckoutRequest**](../Model/CheckoutRequest.md)|  | |

### Return type

[**\MailSafePro\Model\CheckoutSessionResponse**](../Model/CheckoutSessionResponse.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getSubscriptionBillingBillingSubscriptionGet()`

```php
getSubscriptionBillingBillingSubscriptionGet($x_api_key, $authorization): \MailSafePro\Model\SubscriptionResponse
```

Get Subscription

Devuelve información de suscripción (plan y próxima fecha de cobro).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\BillingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$x_api_key = 'x_api_key_example'; // string
$authorization = 'authorization_example'; // string

try {
    $result = $apiInstance->getSubscriptionBillingBillingSubscriptionGet($x_api_key, $authorization);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BillingApi->getSubscriptionBillingBillingSubscriptionGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **x_api_key** | **string**|  | [optional] |
| **authorization** | **string**|  | [optional] |

### Return type

[**\MailSafePro\Model\SubscriptionResponse**](../Model/SubscriptionResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getSubscriptionBillingBillingSubscriptionGet_0()`

```php
getSubscriptionBillingBillingSubscriptionGet_0($x_api_key, $authorization): \MailSafePro\Model\SubscriptionResponse
```

Get Subscription

Devuelve información de suscripción (plan y próxima fecha de cobro).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\BillingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$x_api_key = 'x_api_key_example'; // string
$authorization = 'authorization_example'; // string

try {
    $result = $apiInstance->getSubscriptionBillingBillingSubscriptionGet_0($x_api_key, $authorization);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BillingApi->getSubscriptionBillingBillingSubscriptionGet_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **x_api_key** | **string**|  | [optional] |
| **authorization** | **string**|  | [optional] |

### Return type

[**\MailSafePro\Model\SubscriptionResponse**](../Model/SubscriptionResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stripeWebhookBillingBillingWebhookPost()`

```php
stripeWebhookBillingBillingWebhookPost(): \MailSafePro\Model\WebhookResponse
```

Stripe Webhook

Webhook de Stripe.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\BillingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->stripeWebhookBillingBillingWebhookPost();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BillingApi->stripeWebhookBillingBillingWebhookPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\MailSafePro\Model\WebhookResponse**](../Model/WebhookResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stripeWebhookBillingBillingWebhookPost_0()`

```php
stripeWebhookBillingBillingWebhookPost_0(): \MailSafePro\Model\WebhookResponse
```

Stripe Webhook

Webhook de Stripe.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new MailSafePro\Api\BillingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->stripeWebhookBillingBillingWebhookPost_0();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BillingApi->stripeWebhookBillingBillingWebhookPost_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\MailSafePro\Model\WebhookResponse**](../Model/WebhookResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `testNotificationBillingBillingTestNotificationPost()`

```php
testNotificationBillingBillingTestNotificationPost($request_body): array<string,\MailSafePro\Model\ResponseTestNotificationBillingBillingTestNotificationPostValue>
```

Test Notification

Envía un email de prueba de cambio de plan.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\BillingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$request_body = array('key' => 'request_body_example'); // array<string,string>

try {
    $result = $apiInstance->testNotificationBillingBillingTestNotificationPost($request_body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BillingApi->testNotificationBillingBillingTestNotificationPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **request_body** | [**array<string,string>**](../Model/string.md)|  | |

### Return type

[**array<string,\MailSafePro\Model\ResponseTestNotificationBillingBillingTestNotificationPostValue>**](../Model/ResponseTestNotificationBillingBillingTestNotificationPostValue.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `testNotificationBillingBillingTestNotificationPost_0()`

```php
testNotificationBillingBillingTestNotificationPost_0($request_body): array<string,\MailSafePro\Model\ResponseTestNotificationBillingBillingTestNotificationPostValue>
```

Test Notification

Envía un email de prueba de cambio de plan.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: Bearer
$config = MailSafePro\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new MailSafePro\Api\BillingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$request_body = array('key' => 'request_body_example'); // array<string,string>

try {
    $result = $apiInstance->testNotificationBillingBillingTestNotificationPost_0($request_body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BillingApi->testNotificationBillingBillingTestNotificationPost_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **request_body** | [**array<string,string>**](../Model/string.md)|  | |

### Return type

[**array<string,\MailSafePro\Model\ResponseTestNotificationBillingBillingTestNotificationPostValue>**](../Model/ResponseTestNotificationBillingBillingTestNotificationPostValue.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
