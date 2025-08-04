# GetAccountChanges200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**changes** | Option<[**models::AccountChanges**](AccountChanges.md)> |  | [optional]
**state** | Option<[**models::AccountChangesState**](AccountChangesState.md)> |  | [optional]
**last_transaction_id** | Option<**String**> | The ID of the last Transaction created for the Account.  This Transaction ID should be used for future poll requests, as the client has already observed all changes up to and including it. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


