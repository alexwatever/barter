# OrderFillTransaction

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**String**> | The Transaction's Identifier. | [optional]
**time** | Option<**String**> | The date/time when the Transaction was created. | [optional]
**user_id** | Option<**i32**> | The ID of the user that initiated the creation of the Transaction. | [optional]
**account_id** | Option<**String**> | The ID of the Account the Transaction was created for. | [optional]
**batch_id** | Option<**String**> | The ID of the \"batch\" that the Transaction belongs to. Transactions in the same batch are applied to the Account simultaneously. | [optional]
**request_id** | Option<**String**> | The Request ID of the request which generated the transaction. | [optional]
**r#type** | Option<**String**> | The Type of the Transaction. Always set to \"ORDER_FILL\" for an OrderFillTransaction. | [optional]
**order_id** | Option<**String**> | The ID of the Order filled. | [optional]
**client_order_id** | Option<**String**> | The client Order ID of the Order filled (only provided if the client has assigned one). | [optional]
**instrument** | Option<**String**> | The name of the filled Order's instrument. | [optional]
**units** | Option<**String**> | The number of units filled by the OrderFill. | [optional]
**gain_quote_home_conversion_factor** | Option<**String**> | This is the conversion factor in effect for the Account at the time of the OrderFill for converting any gains realized in Instrument quote units into units of the Account's home currency. | [optional]
**loss_quote_home_conversion_factor** | Option<**String**> | This is the conversion factor in effect for the Account at the time of the OrderFill for converting any losses realized in Instrument quote units into units of the Account's home currency. | [optional]
**price** | Option<**String**> | This field is now deprecated and should no longer be used. The individual tradesClosed, tradeReduced and tradeOpened fields contain the exact/official price each unit was filled at. | [optional]
**full_vwap** | Option<**String**> | The price that all of the units of the OrderFill should have been filled at, in the absence of guaranteed price execution. This factors in the Account's current ClientPrice, used liquidity and the units of the OrderFill only. If no Trades were closed with their price clamped for guaranteed stop loss enforcement, then this value will match the price fields of each Trade opened, closed, and reduced, and they will all be the exact same. | [optional]
**full_price** | Option<[**models::ClientPrice**](ClientPrice.md)> |  | [optional]
**reason** | Option<**String**> | The reason that an Order was filled | [optional]
**pl** | Option<**String**> | The profit or loss incurred when the Order was filled. | [optional]
**financing** | Option<**String**> | The financing paid or collected when the Order was filled. | [optional]
**commission** | Option<**String**> | The commission charged in the Account's home currency as a result of filling the Order. The commission is always represented as a positive quantity of the Account's home currency, however it reduces the balance in the Account. | [optional]
**guaranteed_execution_fee** | Option<**String**> | The total guaranteed execution fees charged for all Trades opened, closed or reduced with guaranteed Stop Loss Orders. | [optional]
**account_balance** | Option<**String**> | The Account's balance after the Order was filled. | [optional]
**trade_opened** | Option<[**models::TradeOpen**](TradeOpen.md)> |  | [optional]
**trades_closed** | Option<[**Vec<models::TradeReduce>**](TradeReduce.md)> | The Trades that were closed when the Order was filled (only provided if filling the Order resulted in a closing open Trades). | [optional]
**trade_reduced** | Option<[**models::TradeReduce**](TradeReduce.md)> |  | [optional]
**half_spread_cost** | Option<**String**> | The half spread cost for the OrderFill, which is the sum of the halfSpreadCost values in the tradeOpened, tradesClosed and tradeReduced fields. This can be a positive or negative value and is represented in the home currency of the Account. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


