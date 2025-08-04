# CloseTrade404Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**order_reject_transaction** | Option<[**models::MarketOrderRejectTransaction**](MarketOrderRejectTransaction.md)> |  | [optional]
**last_transaction_id** | Option<**String**> | The ID of the most recent Transaction created for the Account. Only present if the Account exists. | [optional]
**related_transaction_ids** | Option<**Vec<String>**> | The IDs of all Transactions that were created while satisfying the request. Only present if the Account exists. | [optional]
**error_code** | Option<**String**> | The code of the error that has occurred. This field may not be returned for some errors. | [optional]
**error_message** | Option<**String**> | The human-readable description of the error that has occurred. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


