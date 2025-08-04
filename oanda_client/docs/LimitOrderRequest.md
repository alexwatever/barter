# LimitOrderRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**r#type** | Option<**String**> | The type of the Order to Create. Must be set to \"LIMIT\" when creating a Market Order. | [optional]
**instrument** | Option<**String**> | The Limit Order's Instrument. | [optional]
**units** | Option<**String**> | The quantity requested to be filled by the Limit Order. A posititive number of units results in a long Order, and a negative number of units results in a short Order. | [optional]
**price** | Option<**String**> | The price threshold specified for the Limit Order. The Limit Order will only be filled by a market price that is equal to or better than this price. | [optional]
**time_in_force** | Option<**String**> | The time-in-force requested for the Limit Order. | [optional]
**gtd_time** | Option<**String**> | The date/time when the Limit Order will be cancelled if its timeInForce is \"GTD\". | [optional]
**position_fill** | Option<**String**> | Specification of how Positions in the Account are modified when the Order is filled. | [optional]
**trigger_condition** | Option<**String**> | Specification of which price component should be used when determining if an Order should be triggered and filled. This allows Orders to be triggered based on the bid, ask, mid, default (ask for buy, bid for sell) or inverse (ask for sell, bid for buy) price depending on the desired behaviour. Orders are always filled using their default price component. This feature is only provided through the REST API. Clients who choose to specify a non-default trigger condition will not see it reflected in any of OANDA's proprietary or partner trading platforms, their transaction history or their account statements. OANDA platforms always assume that an Order's trigger condition is set to the default value when indicating the distance from an Order's trigger price, and will always provide the default trigger condition when creating or modifying an Order. A special restriction applies when creating a guaranteed Stop Loss Order. In this case the TriggerCondition value must either be \"DEFAULT\", or the \"natural\" trigger side \"DEFAULT\" results in. So for a Stop Loss Order for a long trade valid values are \"DEFAULT\" and \"BID\", and for short trades \"DEFAULT\" and \"ASK\" are valid. | [optional]
**client_extensions** | Option<[**models::ClientExtensions**](ClientExtensions.md)> |  | [optional]
**take_profit_on_fill** | Option<[**models::TakeProfitDetails**](TakeProfitDetails.md)> |  | [optional]
**stop_loss_on_fill** | Option<[**models::StopLossDetails**](StopLossDetails.md)> |  | [optional]
**trailing_stop_loss_on_fill** | Option<[**models::TrailingStopLossDetails**](TrailingStopLossDetails.md)> |  | [optional]
**trade_client_extensions** | Option<[**models::ClientExtensions**](ClientExtensions.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


