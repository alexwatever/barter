# MarketOrderTransaction

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**String**> | The Transaction's Identifier. | [optional]
**time** | Option<**String**> | The date/time when the Transaction was created. | [optional]
**user_id** | Option<**i32**> | The ID of the user that initiated the creation of the Transaction. | [optional]
**account_id** | Option<**String**> | The ID of the Account the Transaction was created for. | [optional]
**batch_id** | Option<**String**> | The ID of the \"batch\" that the Transaction belongs to. Transactions in the same batch are applied to the Account simultaneously. | [optional]
**request_id** | Option<**String**> | The Request ID of the request which generated the transaction. | [optional]
**r#type** | Option<**String**> | The Type of the Transaction. Always set to \"MARKET_ORDER\" in a MarketOrderTransaction. | [optional]
**instrument** | Option<**String**> | The Market Order's Instrument. | [optional]
**units** | Option<**String**> | The quantity requested to be filled by the Market Order. A posititive number of units results in a long Order, and a negative number of units results in a short Order. | [optional]
**time_in_force** | Option<**String**> | The time-in-force requested for the Market Order. Restricted to FOK or IOC for a MarketOrder. | [optional]
**price_bound** | Option<**String**> | The worst price that the client is willing to have the Market Order filled at. | [optional]
**position_fill** | Option<**String**> | Specification of how Positions in the Account are modified when the Order is filled. | [optional]
**trade_close** | Option<[**models::MarketOrderTradeClose**](MarketOrderTradeClose.md)> |  | [optional]
**long_position_closeout** | Option<[**models::MarketOrderPositionCloseout**](MarketOrderPositionCloseout.md)> |  | [optional]
**short_position_closeout** | Option<[**models::MarketOrderPositionCloseout**](MarketOrderPositionCloseout.md)> |  | [optional]
**margin_closeout** | Option<[**models::MarketOrderMarginCloseout**](MarketOrderMarginCloseout.md)> |  | [optional]
**delayed_trade_close** | Option<[**models::MarketOrderDelayedTradeClose**](MarketOrderDelayedTradeClose.md)> |  | [optional]
**reason** | Option<**String**> | The reason that the Market Order was created | [optional]
**client_extensions** | Option<[**models::ClientExtensions**](ClientExtensions.md)> |  | [optional]
**take_profit_on_fill** | Option<[**models::TakeProfitDetails**](TakeProfitDetails.md)> |  | [optional]
**stop_loss_on_fill** | Option<[**models::StopLossDetails**](StopLossDetails.md)> |  | [optional]
**trailing_stop_loss_on_fill** | Option<[**models::TrailingStopLossDetails**](TrailingStopLossDetails.md)> |  | [optional]
**trade_client_extensions** | Option<[**models::ClientExtensions**](ClientExtensions.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


