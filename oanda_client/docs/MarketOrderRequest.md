# MarketOrderRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**r#type** | Option<**String**> | The type of the Order to Create. Must be set to \"MARKET\" when creating a Market Order. | [optional]
**instrument** | Option<**String**> | The Market Order's Instrument. | [optional]
**units** | Option<**String**> | The quantity requested to be filled by the Market Order. A posititive number of units results in a long Order, and a negative number of units results in a short Order. | [optional]
**time_in_force** | Option<**String**> | The time-in-force requested for the Market Order. Restricted to FOK or IOC for a MarketOrder. | [optional]
**price_bound** | Option<**String**> | The worst price that the client is willing to have the Market Order filled at. | [optional]
**position_fill** | Option<**String**> | Specification of how Positions in the Account are modified when the Order is filled. | [optional]
**client_extensions** | Option<[**models::ClientExtensions**](ClientExtensions.md)> |  | [optional]
**take_profit_on_fill** | Option<[**models::TakeProfitDetails**](TakeProfitDetails.md)> |  | [optional]
**stop_loss_on_fill** | Option<[**models::StopLossDetails**](StopLossDetails.md)> |  | [optional]
**trailing_stop_loss_on_fill** | Option<[**models::TrailingStopLossDetails**](TrailingStopLossDetails.md)> |  | [optional]
**trade_client_extensions** | Option<[**models::ClientExtensions**](ClientExtensions.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


