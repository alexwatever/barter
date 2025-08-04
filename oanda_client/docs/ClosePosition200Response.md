# ClosePosition200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**long_order_create_transaction** | Option<[**models::MarketOrderTransaction**](MarketOrderTransaction.md)> |  | [optional]
**long_order_fill_transaction** | Option<[**models::OrderFillTransaction**](OrderFillTransaction.md)> |  | [optional]
**long_order_cancel_transaction** | Option<[**models::OrderCancelTransaction**](OrderCancelTransaction.md)> |  | [optional]
**short_order_create_transaction** | Option<[**models::MarketOrderTransaction**](MarketOrderTransaction.md)> |  | [optional]
**short_order_fill_transaction** | Option<[**models::OrderFillTransaction**](OrderFillTransaction.md)> |  | [optional]
**short_order_cancel_transaction** | Option<[**models::OrderCancelTransaction**](OrderCancelTransaction.md)> |  | [optional]
**related_transaction_ids** | Option<**Vec<String>**> | The IDs of all Transactions that were created while satisfying the request. | [optional]
**last_transaction_id** | Option<**String**> | The ID of the most recent Transaction created for the Account | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


