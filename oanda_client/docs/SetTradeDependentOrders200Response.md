# SetTradeDependentOrders200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**take_profit_order_cancel_transaction** | Option<[**models::OrderCancelTransaction**](OrderCancelTransaction.md)> |  | [optional]
**take_profit_order_transaction** | Option<[**models::TakeProfitOrderTransaction**](TakeProfitOrderTransaction.md)> |  | [optional]
**take_profit_order_fill_transaction** | Option<[**models::OrderFillTransaction**](OrderFillTransaction.md)> |  | [optional]
**take_profit_order_created_cancel_transaction** | Option<[**models::OrderCancelTransaction**](OrderCancelTransaction.md)> |  | [optional]
**stop_loss_order_cancel_transaction** | Option<[**models::OrderCancelTransaction**](OrderCancelTransaction.md)> |  | [optional]
**stop_loss_order_transaction** | Option<[**models::StopLossOrderTransaction**](StopLossOrderTransaction.md)> |  | [optional]
**stop_loss_order_fill_transaction** | Option<[**models::OrderFillTransaction**](OrderFillTransaction.md)> |  | [optional]
**stop_loss_order_created_cancel_transaction** | Option<[**models::OrderCancelTransaction**](OrderCancelTransaction.md)> |  | [optional]
**trailing_stop_loss_order_cancel_transaction** | Option<[**models::OrderCancelTransaction**](OrderCancelTransaction.md)> |  | [optional]
**trailing_stop_loss_order_transaction** | Option<[**models::TrailingStopLossOrderTransaction**](TrailingStopLossOrderTransaction.md)> |  | [optional]
**related_transaction_ids** | Option<**Vec<String>**> | The IDs of all Transactions that were created while satisfying the request. | [optional]
**last_transaction_id** | Option<**String**> | The ID of the most recent Transaction created for the Account | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


