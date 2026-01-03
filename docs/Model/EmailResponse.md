# # EmailResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **string** | Validated email address |
**valid** | **bool** | Overall validation result |
**detail** | **string** | Validation details summary | [optional] [default to '']
**processing_time** | **float** |  | [optional]
**provider** | **string** |  | [optional]
**reputation** | **float** |  | [optional]
**fingerprint** | **string** |  | [optional]
**quality_score** | **float** |  | [optional]
**risk_level** | [**\MailSafePro\Model\RiskLevelEnum**](RiskLevelEnum.md) |  | [optional]
**suggestions** | **string[]** | Improvement suggestions | [optional]
**smtp** | [**\MailSafePro\Model\SMTPInfo**](SMTPInfo.md) |  | [optional]
**dns** | [**\MailSafePro\Model\DNSInfo**](DNSInfo.md) |  | [optional]
**risk_score** | **float** |  | [optional]
**validation_tier** | **string** |  | [optional]
**suggested_action** | **string** |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
