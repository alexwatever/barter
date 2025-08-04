# ReplaceOrder400Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**order_reject_transaction** | Option<[**models::Transaction**](Transaction.md)> |  | [optional]
**related_transaction_ids** | Option<**Vec<String>**> | The IDs of all Transactions that were created while satisfying the request. | [optional]
**last_transaction_id** | Option<**String**> | The ID of the most recent Transaction created for the Account. | [optional]
**error_code** | Option<**String**> | The code of the error that has occurred. This field may not be returned for some errors. | [optional]
**error_message** | Option<**String**> | The human-readable description of the error that has occurred. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


