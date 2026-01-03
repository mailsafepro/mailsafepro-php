# # APIKeyMeta

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique key identifier |
**key_hash** | **string** | Hashed key value |
**plan** | [**\MailSafePro\Model\PlanEnum**](PlanEnum.md) | Associated plan |
**created_at** | **\DateTime** | Creation timestamp |
**revoked** | **bool** | Revocation status |
**revoked_at** | **\DateTime** |  | [optional]
**scopes** | **string[]** | Access scopes | [optional]
**name** | **string** |  | [optional]
**last_used** | **\DateTime** |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
