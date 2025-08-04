# MarketOrder

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**String**> | The Order's identifier, unique within the Order's Account. | [optional]
**create_time** | Option<**String**> | The time when the Order was created. | [optional]
**state** | Option<**String**> | The current state of the Order. | [optional]
**client_extensions** | Option<[**models::ClientExtensions**](ClientExtensions.md)> |  | [optional]
**r#type** | Option<**String**> | The type of the Order. Always set to \"MARKET\" for Market Orders. | [optional]
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
**take_profit_on_fill** | Option<[**models::TakeProfitDetails**](TakeProfitDetails.md)> |  | [optional]
**stop_loss_on_fill** | Option<[**models::StopLossDetails**](StopLossDetails.md)> |  | [optional]
**trailing_stop_loss_on_fill** | Option<[**models::TrailingStopLossDetails**](TrailingStopLossDetails.md)> |  | [optional]
**trade_client_extensions** | Option<[**models::ClientExtensions**](ClientExtensions.md)> |  | [optional]
**filling_transaction_id** | Option<**String**> | ID of the Transaction that filled this Order (only provided when the Order's state is FILLED) | [optional]
**filled_time** | Option<**String**> | Date/time when the Order was filled (only provided when the Order's state is FILLED) | [optional]
**trade_opened_id** | Option<**String**> | Trade ID of Trade opened when the Order was filled (only provided when the Order's state is FILLED and a Trade was opened as a result of the fill) | [optional]
**trade_reduced_id** | Option<**String**> | Trade ID of Trade reduced when the Order was filled (only provided when the Order's state is FILLED and a Trade was reduced as a result of the fill) | [optional]
**trade_closed_ids** | Option<**Vec<String>**> | Trade IDs of Trades closed when the Order was filled (only provided when the Order's state is FILLED and one or more Trades were closed as a result of the fill) | [optional]
**cancelling_transaction_id** | Option<**String**> | ID of the Transaction that cancelled the Order (only provided when the Order's state is CANCELLED) | [optional]
**cancelled_time** | Option<**String**> | Date/time when the Order was cancelled (only provided when the state of the Order is CANCELLED) | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


