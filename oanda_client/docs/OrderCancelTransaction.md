# OrderCancelTransaction

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**String**> | The Transaction's Identifier. | [optional]
**time** | Option<**String**> | The date/time when the Transaction was created. | [optional]
**user_id** | Option<**i32**> | The ID of the user that initiated the creation of the Transaction. | [optional]
**account_id** | Option<**String**> | The ID of the Account the Transaction was created for. | [optional]
**batch_id** | Option<**String**> | The ID of the \"batch\" that the Transaction belongs to. Transactions in the same batch are applied to the Account simultaneously. | [optional]
**request_id** | Option<**String**> | The Request ID of the request which generated the transaction. | [optional]
**r#type** | Option<**String**> | The Type of the Transaction. Always set to \"ORDER_CANCEL\" for an OrderCancelTransaction. | [optional]
**order_id** | Option<**String**> | The ID of the Order cancelled | [optional]
**client_order_id** | Option<**String**> | The client ID of the Order cancelled (only provided if the Order has a client Order ID). | [optional]
**reason** | Option<**String**> | The reason that the Order was cancelled. | [optional]
**replaced_by_order_id** | Option<**String**> | The ID of the Order that replaced this Order (only provided if this Order was cancelled for replacement). | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


