# # BatchValidationRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**emails** | **string[]** | List of email addresses to validate (can include invalid formats) |
**check_smtp** | **bool** | Perform SMTP verification for all emails | [optional] [default to false]
**include_raw_dns** | **bool** | Include raw DNS records in responses | [optional] [default to false]
**batch_size** | **int** | Number of emails to process in each batch | [optional] [default to 100]
**concurrent_requests** | **int** | Maximum concurrent validation requests | [optional] [default to 5]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
