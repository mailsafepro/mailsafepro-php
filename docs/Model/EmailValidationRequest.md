# # EmailValidationRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **string** | Email address to validate (RFC 5321 compliant) |
**check_smtp** | **bool** | Enable SMTP mailbox verification | [optional] [default to false]
**include_raw_dns** | **bool** | Include raw DNS records | [optional] [default to false]
**testing_mode** | **bool** | Enable testing mode (allows special TLDs like .test, .example, etc.) | [optional] [default to false]
**priority** | [**\MailSafePro\Model\PriorityEnum**](PriorityEnum.md) | Validation priority level | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
