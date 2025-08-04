# Trade

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**String**> | The Trade's identifier, unique within the Trade's Account. | [optional]
**instrument** | Option<**String**> | The Trade's Instrument. | [optional]
**price** | Option<**String**> | The execution price of the Trade. | [optional]
**open_time** | Option<**String**> | The date/time when the Trade was opened. | [optional]
**state** | Option<**String**> | The current state of the Trade. | [optional]
**initial_units** | Option<**String**> | The initial size of the Trade. Negative values indicate a short Trade, and positive values indicate a long Trade. | [optional]
**initial_margin_required** | Option<**String**> | The margin required at the time the Trade was created. Note, this is the 'pure' margin required, it is not the 'effective' margin used that factors in the trade risk if a GSLO is attached to the trade. | [optional]
**current_units** | Option<**String**> | The number of units currently open for the Trade. This value is reduced to 0.0 as the Trade is closed. | [optional]
**realized_pl** | Option<**String**> | The total profit/loss realized on the closed portion of the Trade. | [optional]
**unrealized_pl** | Option<**String**> | The unrealized profit/loss on the open portion of the Trade. | [optional]
**margin_used** | Option<**String**> | Margin currently used by the Trade. | [optional]
**average_close_price** | Option<**String**> | The average closing price of the Trade. Only present if the Trade has been closed or reduced at least once. | [optional]
**closing_transaction_ids** | Option<**Vec<String>**> | The IDs of the Transactions that have closed portions of this Trade. | [optional]
**financing** | Option<**String**> | The financing paid/collected for this Trade. | [optional]
**close_time** | Option<**String**> | The date/time when the Trade was fully closed. Only provided for Trades whose state is CLOSED. | [optional]
**client_extensions** | Option<[**models::ClientExtensions**](ClientExtensions.md)> |  | [optional]
**take_profit_order** | Option<[**models::TakeProfitOrder**](TakeProfitOrder.md)> |  | [optional]
**stop_loss_order** | Option<[**models::StopLossOrder**](StopLossOrder.md)> |  | [optional]
**trailing_stop_loss_order** | Option<[**models::TrailingStopLossOrder**](TrailingStopLossOrder.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


