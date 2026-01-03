# mailsafepro

API robusta y segura para validación y verificación de correos electrónicos.
Soporta verificación individual y en lote, detección de brechas, y autenticación JWT.
Cumple con GDPR y dispone de planes de pago flexibles.

**🔗 Enlaces importantes:**
- [Estado del sistema](https://mailsafepro.betteruptime.com)
- [Documentación completa](https://email-validation-api-jlra.onrender.com/redoc)

**📧 Contacto:** mailsafepro1@gmail.com


## Installation & Usage

### Requirements

PHP 8.1 and later.

### Composer

To install the bindings via [Composer](https://getcomposer.org/), add the following to `composer.json`:

```json
{
  "repositories": [
    {
      "type": "vcs",
      "url": "https://github.com/mailsafepro/mailsafepro-php.git"
    }
  ],
  "require": {
    "mailsafepro/mailsafepro-php": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
<?php
require_once('/path/to/mailsafepro/vendor/autoload.php');
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

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

## API Endpoints

All URIs are relative to *http://localhost*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*APIKeysApi* | [**createApiKeyApiKeysPost**](docs/Api/APIKeysApi.md#createapikeyapikeyspost) | **POST** /api-keys | Create Api Key
*APIKeysApi* | [**createApiKeyApiKeysPost_0**](docs/Api/APIKeysApi.md#createapikeyapikeyspost_0) | **POST** /api-keys | Create Api Key
*APIKeysApi* | [**forceSyncApiKeysForceSyncPost**](docs/Api/APIKeysApi.md#forcesyncapikeysforcesyncpost) | **POST** /api-keys/force-sync | Force Sync
*APIKeysApi* | [**forceSyncApiKeysForceSyncPost_0**](docs/Api/APIKeysApi.md#forcesyncapikeysforcesyncpost_0) | **POST** /api-keys/force-sync | Force Sync
*APIKeysApi* | [**getApiKeyValueApiKeysKeyHashValueGet**](docs/Api/APIKeysApi.md#getapikeyvalueapikeyskeyhashvalueget) | **GET** /api-keys/{key_hash}/value | Get Api Key Value
*APIKeysApi* | [**getApiKeyValueApiKeysKeyHashValueGet_0**](docs/Api/APIKeysApi.md#getapikeyvalueapikeyskeyhashvalueget_0) | **GET** /api-keys/{key_hash}/value | Get Api Key Value
*APIKeysApi* | [**getUsageApiKeysUsageGet**](docs/Api/APIKeysApi.md#getusageapikeysusageget) | **GET** /api-keys/usage | Get Usage
*APIKeysApi* | [**getUsageApiKeysUsageGet_0**](docs/Api/APIKeysApi.md#getusageapikeysusageget_0) | **GET** /api-keys/usage | Get Usage
*APIKeysApi* | [**listApiKeysApiKeysGet**](docs/Api/APIKeysApi.md#listapikeysapikeysget) | **GET** /api-keys | List Api Keys
*APIKeysApi* | [**listApiKeysApiKeysGet_0**](docs/Api/APIKeysApi.md#listapikeysapikeysget_0) | **GET** /api-keys | List Api Keys
*APIKeysApi* | [**repairUserDataEndpointApiKeysRepairDataPost**](docs/Api/APIKeysApi.md#repairuserdataendpointapikeysrepairdatapost) | **POST** /api-keys/repair-data | Repair User Data Endpoint
*APIKeysApi* | [**repairUserDataEndpointApiKeysRepairDataPost_0**](docs/Api/APIKeysApi.md#repairuserdataendpointapikeysrepairdatapost_0) | **POST** /api-keys/repair-data | Repair User Data Endpoint
*APIKeysApi* | [**revokeApiKeyApiKeysKeyHashRevokeDelete**](docs/Api/APIKeysApi.md#revokeapikeyapikeyskeyhashrevokedelete) | **DELETE** /api-keys/{key_hash}/revoke | Revoke Api Key
*APIKeysApi* | [**revokeApiKeyApiKeysKeyHashRevokeDelete_0**](docs/Api/APIKeysApi.md#revokeapikeyapikeyskeyhashrevokedelete_0) | **DELETE** /api-keys/{key_hash}/revoke | Revoke Api Key
*APIKeysApi* | [**rotateApiKeyApiKeysKeyHashRotatePost**](docs/Api/APIKeysApi.md#rotateapikeyapikeyskeyhashrotatepost) | **POST** /api-keys/{key_hash}/rotate | Rotate Api Key
*APIKeysApi* | [**rotateApiKeyApiKeysKeyHashRotatePost_0**](docs/Api/APIKeysApi.md#rotateapikeyapikeyskeyhashrotatepost_0) | **POST** /api-keys/{key_hash}/rotate | Rotate Api Key
*APIKeysApi* | [**syncPlanKeysApiKeysSyncPlanKeysPost**](docs/Api/APIKeysApi.md#syncplankeysapikeyssyncplankeyspost) | **POST** /api-keys/sync-plan-keys | Sync Plan Keys
*APIKeysApi* | [**syncPlanKeysApiKeysSyncPlanKeysPost_0**](docs/Api/APIKeysApi.md#syncplankeysapikeyssyncplankeyspost_0) | **POST** /api-keys/sync-plan-keys | Sync Plan Keys
*AuthenticationApi* | [**authHealthCheckAuthHealthAuthGet**](docs/Api/AuthenticationApi.md#authhealthcheckauthhealthauthget) | **GET** /auth/health/auth | Auth Health Check
*AuthenticationApi* | [**authHealthCheckAuthHealthAuthGet_0**](docs/Api/AuthenticationApi.md#authhealthcheckauthhealthauthget_0) | **GET** /auth/health/auth | Auth Health Check
*AuthenticationApi* | [**authHealthCheckAuthHealthAuthHead**](docs/Api/AuthenticationApi.md#authhealthcheckauthhealthauthhead) | **HEAD** /auth/health/auth | Auth Health Check
*AuthenticationApi* | [**authHealthCheckAuthHealthAuthHead_0**](docs/Api/AuthenticationApi.md#authhealthcheckauthhealthauthhead_0) | **HEAD** /auth/health/auth | Auth Health Check
*AuthenticationApi* | [**deleteAccountAuthDeleteDelete**](docs/Api/AuthenticationApi.md#deleteaccountauthdeletedelete) | **DELETE** /auth/delete | Delete Account
*AuthenticationApi* | [**deleteAccountAuthDeleteDelete_0**](docs/Api/AuthenticationApi.md#deleteaccountauthdeletedelete_0) | **DELETE** /auth/delete | Delete Account
*AuthenticationApi* | [**getCurrentUserAuthMeGet**](docs/Api/AuthenticationApi.md#getcurrentuserauthmeget) | **GET** /auth/me | Get Current User
*AuthenticationApi* | [**getCurrentUserAuthMeGet_0**](docs/Api/AuthenticationApi.md#getcurrentuserauthmeget_0) | **GET** /auth/me | Get Current User
*AuthenticationApi* | [**loginWebUserAuthLoginPost**](docs/Api/AuthenticationApi.md#loginwebuserauthloginpost) | **POST** /auth/login | Login Web User
*AuthenticationApi* | [**loginWebUserAuthLoginPost_0**](docs/Api/AuthenticationApi.md#loginwebuserauthloginpost_0) | **POST** /auth/login | Login Web User
*AuthenticationApi* | [**logoutAuthLogoutPost**](docs/Api/AuthenticationApi.md#logoutauthlogoutpost) | **POST** /auth/logout | Logout
*AuthenticationApi* | [**logoutAuthLogoutPost_0**](docs/Api/AuthenticationApi.md#logoutauthlogoutpost_0) | **POST** /auth/logout | Logout
*AuthenticationApi* | [**refreshTokenAuthRefreshPost**](docs/Api/AuthenticationApi.md#refreshtokenauthrefreshpost) | **POST** /auth/refresh | Refresh Token
*AuthenticationApi* | [**refreshTokenAuthRefreshPost_0**](docs/Api/AuthenticationApi.md#refreshtokenauthrefreshpost_0) | **POST** /auth/refresh | Refresh Token
*AuthenticationApi* | [**registerWebUserAuthRegisterPost**](docs/Api/AuthenticationApi.md#registerwebuserauthregisterpost) | **POST** /auth/register | Register Web User
*AuthenticationApi* | [**registerWebUserAuthRegisterPost_0**](docs/Api/AuthenticationApi.md#registerwebuserauthregisterpost_0) | **POST** /auth/register | Register Web User
*AuthenticationApi* | [**rotateApiKeyAuthRotateKeyPost**](docs/Api/AuthenticationApi.md#rotateapikeyauthrotatekeypost) | **POST** /auth/rotate-key | Rotate Api Key
*AuthenticationApi* | [**rotateApiKeyAuthRotateKeyPost_0**](docs/Api/AuthenticationApi.md#rotateapikeyauthrotatekeypost_0) | **POST** /auth/rotate-key | Rotate Api Key
*BillingApi* | [**changePlanBillingBillingChangePlanPost**](docs/Api/BillingApi.md#changeplanbillingbillingchangeplanpost) | **POST** /billing/billing/change-plan | Change Plan
*BillingApi* | [**changePlanBillingBillingChangePlanPost_0**](docs/Api/BillingApi.md#changeplanbillingbillingchangeplanpost_0) | **POST** /billing/billing/change-plan | Change Plan
*BillingApi* | [**createCheckoutSessionBillingBillingCreateCheckoutSessionPost**](docs/Api/BillingApi.md#createcheckoutsessionbillingbillingcreatecheckoutsessionpost) | **POST** /billing/billing/create-checkout-session | Create Checkout Session
*BillingApi* | [**createCheckoutSessionBillingBillingCreateCheckoutSessionPost_0**](docs/Api/BillingApi.md#createcheckoutsessionbillingbillingcreatecheckoutsessionpost_0) | **POST** /billing/billing/create-checkout-session | Create Checkout Session
*BillingApi* | [**getSubscriptionBillingBillingSubscriptionGet**](docs/Api/BillingApi.md#getsubscriptionbillingbillingsubscriptionget) | **GET** /billing/billing/subscription | Get Subscription
*BillingApi* | [**getSubscriptionBillingBillingSubscriptionGet_0**](docs/Api/BillingApi.md#getsubscriptionbillingbillingsubscriptionget_0) | **GET** /billing/billing/subscription | Get Subscription
*BillingApi* | [**stripeWebhookBillingBillingWebhookPost**](docs/Api/BillingApi.md#stripewebhookbillingbillingwebhookpost) | **POST** /billing/billing/webhook | Stripe Webhook
*BillingApi* | [**stripeWebhookBillingBillingWebhookPost_0**](docs/Api/BillingApi.md#stripewebhookbillingbillingwebhookpost_0) | **POST** /billing/billing/webhook | Stripe Webhook
*BillingApi* | [**testNotificationBillingBillingTestNotificationPost**](docs/Api/BillingApi.md#testnotificationbillingbillingtestnotificationpost) | **POST** /billing/billing/test-notification | Test Notification
*BillingApi* | [**testNotificationBillingBillingTestNotificationPost_0**](docs/Api/BillingApi.md#testnotificationbillingbillingtestnotificationpost_0) | **POST** /billing/billing/test-notification | Test Notification
*DefaultApi* | [**askGeminiGeminiGet**](docs/Api/DefaultApi.md#askgeminigeminiget) | **GET** /gemini | Ask Gemini
*DefaultApi* | [**runAuditAdminAuditProjectPost**](docs/Api/DefaultApi.md#runauditadminauditprojectpost) | **POST** /admin/audit_project | Run Audit
*DeveloperToolsApi* | [**clearRequestLogsLogsLogsRequestsDelete**](docs/Api/DeveloperToolsApi.md#clearrequestlogslogslogsrequestsdelete) | **DELETE** /logs/logs/requests | Clear Request Logs
*DeveloperToolsApi* | [**getRequestLogsLogsLogsRequestsGet**](docs/Api/DeveloperToolsApi.md#getrequestlogslogslogsrequestsget) | **GET** /logs/logs/requests | Get Request Logs
*EmailValidationApi* | [**batchValidateEmailsValidateBatchPost**](docs/Api/EmailValidationApi.md#batchvalidateemailsvalidatebatchpost) | **POST** /validate/batch | Batch Email Validation
*EmailValidationApi* | [**batchValidateUploadValidateBatchUploadPost**](docs/Api/EmailValidationApi.md#batchvalidateuploadvalidatebatchuploadpost) | **POST** /validate/batch/upload | Batch Email Validation via File Upload
*EmailValidationApi* | [**getCacheStatsValidateStatsCacheGet**](docs/Api/EmailValidationApi.md#getcachestatsvalidatestatscacheget) | **GET** /validate/stats/cache | Get Cache Stats
*EmailValidationApi* | [**getUsageStatsValidateStatsUsageGet**](docs/Api/EmailValidationApi.md#getusagestatsvalidatestatsusageget) | **GET** /validate/stats/usage | Get Usage Stats
*EmailValidationApi* | [**healthCheckValidateHealthGet**](docs/Api/EmailValidationApi.md#healthcheckvalidatehealthget) | **GET** /validate/health | Health Check
*EmailValidationApi* | [**healthCheckValidateHealthHead**](docs/Api/EmailValidationApi.md#healthcheckvalidatehealthhead) | **HEAD** /validate/health | Health Check
*EmailValidationApi* | [**validateEmailEndpointValidateEmailPost**](docs/Api/EmailValidationApi.md#validateemailendpointvalidateemailpost) | **POST** /validate/email | Validate Email Endpoint
*HealthApi* | [**basicHealthHealthGet**](docs/Api/HealthApi.md#basichealthhealthget) | **GET** /health | Basic health check
*HealthApi* | [**basicHealthHealthGet_0**](docs/Api/HealthApi.md#basichealthhealthget_0) | **GET** /health | Basic health check
*HealthApi* | [**circuitBreakerStatusAdminCircuitBreakerStatusGet**](docs/Api/HealthApi.md#circuitbreakerstatusadmincircuitbreakerstatusget) | **GET** /admin/circuit-breaker-status | Circuit Breaker Status
*HealthApi* | [**detailedHealthHealthDetailedGet**](docs/Api/HealthApi.md#detailedhealthhealthdetailedget) | **GET** /health/detailed | Detailed health check
*HealthApi* | [**detailedHealthHealthDetailedGet_0**](docs/Api/HealthApi.md#detailedhealthhealthdetailedget_0) | **GET** /health/detailed | Detailed health check
*HealthApi* | [**healthcheckHealthcheckGet**](docs/Api/HealthApi.md#healthcheckhealthcheckget) | **GET** /healthcheck | Healthcheck
*HealthApi* | [**healthcheckHealthcheckHead**](docs/Api/HealthApi.md#healthcheckhealthcheckhead) | **HEAD** /healthcheck | Healthcheck
*HealthApi* | [**livenessCheckHealthLivenessGet**](docs/Api/HealthApi.md#livenesscheckhealthlivenessget) | **GET** /health/liveness | Liveness Check
*HealthApi* | [**livenessHealthLiveGet**](docs/Api/HealthApi.md#livenesshealthliveget) | **GET** /health/live | Liveness probe (Kubernetes)
*HealthApi* | [**livenessHealthLiveGet_0**](docs/Api/HealthApi.md#livenesshealthliveget_0) | **GET** /health/live | Liveness probe (Kubernetes)
*HealthApi* | [**readinessCheckHealthReadinessGet**](docs/Api/HealthApi.md#readinesscheckhealthreadinessget) | **GET** /health/readiness | Readiness Check
*HealthApi* | [**readinessHealthReadyGet**](docs/Api/HealthApi.md#readinesshealthreadyget) | **GET** /health/ready | Readiness probe (Kubernetes)
*HealthApi* | [**readinessHealthReadyGet_0**](docs/Api/HealthApi.md#readinesshealthreadyget_0) | **GET** /health/ready | Readiness probe (Kubernetes)
*HealthApi* | [**serviceStatusStatusGet**](docs/Api/HealthApi.md#servicestatusstatusget) | **GET** /status | Service Status
*HealthApi* | [**startupCheckHealthStartupGet**](docs/Api/HealthApi.md#startupcheckhealthstartupget) | **GET** /health/startup | Startup Check
*JobsApi* | [**createJobJobsV1JobsPost**](docs/Api/JobsApi.md#createjobjobsv1jobspost) | **POST** /jobs/v1/jobs | Create validation job
*JobsApi* | [**createJobJobsV1JobsPost_0**](docs/Api/JobsApi.md#createjobjobsv1jobspost_0) | **POST** /jobs/v1/jobs | Create validation job
*JobsApi* | [**getJobResultsJobsV1JobsJobIdResultsGet**](docs/Api/JobsApi.md#getjobresultsjobsv1jobsjobidresultsget) | **GET** /jobs/v1/jobs/{job_id}/results | Get job results (paged)
*JobsApi* | [**getJobResultsJobsV1JobsJobIdResultsGet_0**](docs/Api/JobsApi.md#getjobresultsjobsv1jobsjobidresultsget_0) | **GET** /jobs/v1/jobs/{job_id}/results | Get job results (paged)
*JobsApi* | [**getJobStatusJobsV1JobsJobIdGet**](docs/Api/JobsApi.md#getjobstatusjobsv1jobsjobidget) | **GET** /jobs/v1/jobs/{job_id} | Get job status
*JobsApi* | [**getJobStatusJobsV1JobsJobIdGet_0**](docs/Api/JobsApi.md#getjobstatusjobsv1jobsjobidget_0) | **GET** /jobs/v1/jobs/{job_id} | Get job status
*LogsApi* | [**clearRequestLogsLogsLogsRequestsDelete**](docs/Api/LogsApi.md#clearrequestlogslogslogsrequestsdelete) | **DELETE** /logs/logs/requests | Clear Request Logs
*LogsApi* | [**getRequestLogsLogsLogsRequestsGet**](docs/Api/LogsApi.md#getrequestlogslogslogsrequestsget) | **GET** /logs/logs/requests | Get Request Logs
*ValidationApi* | [**batchValidateEmailsValidateBatchPost**](docs/Api/ValidationApi.md#batchvalidateemailsvalidatebatchpost) | **POST** /validate/batch | Batch Email Validation
*ValidationApi* | [**batchValidateUploadValidateBatchUploadPost**](docs/Api/ValidationApi.md#batchvalidateuploadvalidatebatchuploadpost) | **POST** /validate/batch/upload | Batch Email Validation via File Upload
*ValidationApi* | [**getCacheStatsValidateStatsCacheGet**](docs/Api/ValidationApi.md#getcachestatsvalidatestatscacheget) | **GET** /validate/stats/cache | Get Cache Stats
*ValidationApi* | [**getUsageStatsValidateStatsUsageGet**](docs/Api/ValidationApi.md#getusagestatsvalidatestatsusageget) | **GET** /validate/stats/usage | Get Usage Stats
*ValidationApi* | [**healthCheckValidateHealthGet**](docs/Api/ValidationApi.md#healthcheckvalidatehealthget) | **GET** /validate/health | Health Check
*ValidationApi* | [**healthCheckValidateHealthHead**](docs/Api/ValidationApi.md#healthcheckvalidatehealthhead) | **HEAD** /validate/health | Health Check
*ValidationApi* | [**validateEmailEndpointValidateEmailPost**](docs/Api/ValidationApi.md#validateemailendpointvalidateemailpost) | **POST** /validate/email | Validate Email Endpoint
*WebhooksApi* | [**createWebhookWebhooksManagementWebhooksPost**](docs/Api/WebhooksApi.md#createwebhookwebhooksmanagementwebhookspost) | **POST** /webhooks-management/webhooks/ | Create Webhook
*WebhooksApi* | [**deleteWebhookWebhooksManagementWebhooksWebhookIdDelete**](docs/Api/WebhooksApi.md#deletewebhookwebhooksmanagementwebhookswebhookiddelete) | **DELETE** /webhooks-management/webhooks/{webhook_id} | Delete Webhook
*WebhooksApi* | [**getDeliveriesWebhooksManagementWebhooksWebhookIdDeliveriesGet**](docs/Api/WebhooksApi.md#getdeliverieswebhooksmanagementwebhookswebhookiddeliveriesget) | **GET** /webhooks-management/webhooks/{webhook_id}/deliveries | Get Deliveries
*WebhooksApi* | [**getWebhookWebhooksManagementWebhooksWebhookIdGet**](docs/Api/WebhooksApi.md#getwebhookwebhooksmanagementwebhookswebhookidget) | **GET** /webhooks-management/webhooks/{webhook_id} | Get Webhook
*WebhooksApi* | [**listWebhooksWebhooksManagementWebhooksGet**](docs/Api/WebhooksApi.md#listwebhookswebhooksmanagementwebhooksget) | **GET** /webhooks-management/webhooks/ | List Webhooks
*WebhooksApi* | [**registerEndpointWebhooksV1WebhooksEndpointsRegisterPost**](docs/Api/WebhooksApi.md#registerendpointwebhooksv1webhooksendpointsregisterpost) | **POST** /webhooks/v1/webhooks/endpoints/register | Register Endpoint
*WebhooksApi* | [**registerEndpointWebhooksV1WebhooksEndpointsRegisterPost_0**](docs/Api/WebhooksApi.md#registerendpointwebhooksv1webhooksendpointsregisterpost_0) | **POST** /webhooks/v1/webhooks/endpoints/register | Register Endpoint
*WebhooksApi* | [**rotateSecretWebhooksV1WebhooksEndpointsRotatePost**](docs/Api/WebhooksApi.md#rotatesecretwebhooksv1webhooksendpointsrotatepost) | **POST** /webhooks/v1/webhooks/endpoints/rotate | Rotate Secret
*WebhooksApi* | [**rotateSecretWebhooksV1WebhooksEndpointsRotatePost_0**](docs/Api/WebhooksApi.md#rotatesecretwebhooksv1webhooksendpointsrotatepost_0) | **POST** /webhooks/v1/webhooks/endpoints/rotate | Rotate Secret
*WebhooksApi* | [**testWebhookWebhooksManagementWebhooksWebhookIdTestPost**](docs/Api/WebhooksApi.md#testwebhookwebhooksmanagementwebhookswebhookidtestpost) | **POST** /webhooks-management/webhooks/{webhook_id}/test | Test Webhook
*WebhooksApi* | [**updateWebhookWebhooksManagementWebhooksWebhookIdPatch**](docs/Api/WebhooksApi.md#updatewebhookwebhooksmanagementwebhookswebhookidpatch) | **PATCH** /webhooks-management/webhooks/{webhook_id} | Update Webhook
*WebhooksManagementApi* | [**createWebhookWebhooksManagementWebhooksPost**](docs/Api/WebhooksManagementApi.md#createwebhookwebhooksmanagementwebhookspost) | **POST** /webhooks-management/webhooks/ | Create Webhook
*WebhooksManagementApi* | [**deleteWebhookWebhooksManagementWebhooksWebhookIdDelete**](docs/Api/WebhooksManagementApi.md#deletewebhookwebhooksmanagementwebhookswebhookiddelete) | **DELETE** /webhooks-management/webhooks/{webhook_id} | Delete Webhook
*WebhooksManagementApi* | [**getDeliveriesWebhooksManagementWebhooksWebhookIdDeliveriesGet**](docs/Api/WebhooksManagementApi.md#getdeliverieswebhooksmanagementwebhookswebhookiddeliveriesget) | **GET** /webhooks-management/webhooks/{webhook_id}/deliveries | Get Deliveries
*WebhooksManagementApi* | [**getWebhookWebhooksManagementWebhooksWebhookIdGet**](docs/Api/WebhooksManagementApi.md#getwebhookwebhooksmanagementwebhookswebhookidget) | **GET** /webhooks-management/webhooks/{webhook_id} | Get Webhook
*WebhooksManagementApi* | [**listWebhooksWebhooksManagementWebhooksGet**](docs/Api/WebhooksManagementApi.md#listwebhookswebhooksmanagementwebhooksget) | **GET** /webhooks-management/webhooks/ | List Webhooks
*WebhooksManagementApi* | [**testWebhookWebhooksManagementWebhooksWebhookIdTestPost**](docs/Api/WebhooksManagementApi.md#testwebhookwebhooksmanagementwebhookswebhookidtestpost) | **POST** /webhooks-management/webhooks/{webhook_id}/test | Test Webhook
*WebhooksManagementApi* | [**updateWebhookWebhooksManagementWebhooksWebhookIdPatch**](docs/Api/WebhooksManagementApi.md#updatewebhookwebhooksmanagementwebhookswebhookidpatch) | **PATCH** /webhooks-management/webhooks/{webhook_id} | Update Webhook

## Models

- [APIKeyCreateRequest](docs/Model/APIKeyCreateRequest.md)
- [APIKeyListResponse](docs/Model/APIKeyListResponse.md)
- [APIKeyMeta](docs/Model/APIKeyMeta.md)
- [BatchEmailResponse](docs/Model/BatchEmailResponse.md)
- [BatchValidationRequest](docs/Model/BatchValidationRequest.md)
- [BodyChangePlanBillingBillingChangePlanPost](docs/Model/BodyChangePlanBillingBillingChangePlanPost.md)
- [CheckoutRequest](docs/Model/CheckoutRequest.md)
- [CheckoutSessionResponse](docs/Model/CheckoutSessionResponse.md)
- [DNSInfo](docs/Model/DNSInfo.md)
- [DNSRecordDKIM](docs/Model/DNSRecordDKIM.md)
- [DNSRecordDMARC](docs/Model/DNSRecordDMARC.md)
- [DNSRecordSPF](docs/Model/DNSRecordSPF.md)
- [EmailResponse](docs/Model/EmailResponse.md)
- [EmailValidationRequest](docs/Model/EmailValidationRequest.md)
- [HTTPValidationError](docs/Model/HTTPValidationError.md)
- [JobCreateRequest](docs/Model/JobCreateRequest.md)
- [JobCreateResponse](docs/Model/JobCreateResponse.md)
- [JobResultEntry](docs/Model/JobResultEntry.md)
- [JobResultsPage](docs/Model/JobResultsPage.md)
- [JobStatusResponse](docs/Model/JobStatusResponse.md)
- [KeyRotationRequest](docs/Model/KeyRotationRequest.md)
- [PlanEnum](docs/Model/PlanEnum.md)
- [PriorityEnum](docs/Model/PriorityEnum.md)
- [RegisterEndpoint](docs/Model/RegisterEndpoint.md)
- [ResponseTestNotificationBillingBillingTestNotificationPostValue](docs/Model/ResponseTestNotificationBillingBillingTestNotificationPostValue.md)
- [RiskLevelEnum](docs/Model/RiskLevelEnum.md)
- [RotateSecret](docs/Model/RotateSecret.md)
- [SMTPInfo](docs/Model/SMTPInfo.md)
- [SubscriptionResponse](docs/Model/SubscriptionResponse.md)
- [UserLogin](docs/Model/UserLogin.md)
- [UserRegister](docs/Model/UserRegister.md)
- [ValidationError](docs/Model/ValidationError.md)
- [ValidationErrorLocInner](docs/Model/ValidationErrorLocInner.md)
- [WebhookCreate](docs/Model/WebhookCreate.md)
- [WebhookResponse](docs/Model/WebhookResponse.md)
- [WebhookUpdate](docs/Model/WebhookUpdate.md)

## Authorization

Authentication schemes defined for the API:
### Bearer

- **Type**: Bearer authentication (JWT)

### ApiKeyAuth

- **Type**: API key
- **API key parameter name**: X-API-Key
- **Location**: HTTP header


## Tests

To run the tests, use:

```bash
composer install
vendor/bin/phpunit
```

## Author



## About this package

This PHP package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: `2.5.0`
    - Package version: `1.0.0`
    - Generator version: `7.18.0`
- Build package: `org.openapitools.codegen.languages.PhpClientCodegen`
