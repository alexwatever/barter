# TrailingStopLossOrderRejectTransaction

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**String**> | The Transaction's Identifier. | [optional]
**time** | Option<**String**> | The date/time when the Transaction was created. | [optional]
**user_id** | Option<**i32**> | The ID of the user that initiated the creation of the Transaction. | [optional]
**account_id** | Option<**String**> | The ID of the Account the Transaction was created for. | [optional]
**batch_id** | Option<**String**> | The ID of the \"batch\" that the Transaction belongs to. Transactions in the same batch are applied to the Account simultaneously. | [optional]
**request_id** | Option<**String**> | The Request ID of the request which generated the transaction. | [optional]
**r#type** | Option<**String**> | The Type of the Transaction. Always set to \"TRAILING_STOP_LOSS_ORDER_REJECT\" in a TrailingStopLossOrderRejectTransaction. | [optional]
**trade_id** | Option<**String**> | The ID of the Trade to close when the price threshold is breached. | [optional]
**client_trade_id** | Option<**String**> | The client ID of the Trade to be closed when the price threshold is breached. | [optional]
**distance** | Option<**String**> | The price distance (in price units) specified for the TrailingStopLoss Order. | [optional]
**time_in_force** | Option<**String**> | The time-in-force requested for the TrailingStopLoss Order. Restricted to \"GTC\", \"GFD\" and \"GTD\" for TrailingStopLoss Orders. | [optional]
**gtd_time** | Option<**String**> | The date/time when the StopLoss Order will be cancelled if its timeInForce is \"GTD\". | [optional]
**trigger_condition** | Option<**String**> | Specification of which price component should be used when determining if an Order should be triggered and filled. This allows Orders to be triggered based on the bid, ask, mid, default (ask for buy, bid for sell) or inverse (ask for sell, bid for buy) price depending on the desired behaviour. Orders are always filled using their default price component. This feature is only provided through the REST API. Clients who choose to specify a non-default trigger condition will not see it reflected in any of OANDA's proprietary or partner trading platforms, their transaction history or their account statements. OANDA platforms always assume that an Order's trigger condition is set to the default value when indicating the distance from an Order's trigger price, and will always provide the default trigger condition when creating or modifying an Order. A special restriction applies when creating a guaranteed Stop Loss Order. In this case the TriggerCondition value must either be \"DEFAULT\", or the \"natural\" trigger side \"DEFAULT\" results in. So for a Stop Loss Order for a long trade valid values are \"DEFAULT\" and \"BID\", and for short trades \"DEFAULT\" and \"ASK\" are valid. | [optional]
**reason** | Option<**String**> | The reason that the Trailing Stop Loss Order was initiated | [optional]
**client_extensions** | Option<[**models::ClientExtensions**](ClientExtensions.md)> |  | [optional]
**order_fill_transaction_id** | Option<**String**> | The ID of the OrderFill Transaction that caused this Order to be created (only provided if this Order was created automatically when another Order was filled). | [optional]
**intended_replaces_order_id** | Option<**String**> | The ID of the Order that this Order was intended to replace (only provided if this Order was intended to replace an existing Order). | [optional]
**reject_reason** | Option<**String**> | The reason that the Reject Transaction was created | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


