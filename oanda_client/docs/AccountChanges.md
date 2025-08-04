# AccountChanges

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**orders_created** | Option<[**Vec<models::Order>**](Order.md)> | The Orders created. These Orders may have been filled, cancelled or triggered in the same period. | [optional]
**orders_cancelled** | Option<[**Vec<models::Order>**](Order.md)> | The Orders cancelled. | [optional]
**orders_filled** | Option<[**Vec<models::Order>**](Order.md)> | The Orders filled. | [optional]
**orders_triggered** | Option<[**Vec<models::Order>**](Order.md)> | The Orders triggered. | [optional]
**trades_opened** | Option<[**Vec<models::TradeSummary>**](TradeSummary.md)> | The Trades opened. | [optional]
**trades_reduced** | Option<[**Vec<models::TradeSummary>**](TradeSummary.md)> | The Trades reduced. | [optional]
**trades_closed** | Option<[**Vec<models::TradeSummary>**](TradeSummary.md)> | The Trades closed. | [optional]
**positions** | Option<[**Vec<models::Position>**](Position.md)> | The Positions changed. | [optional]
**transactions** | Option<[**Vec<models::Transaction>**](Transaction.md)> | The Transactions that have been generated. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


