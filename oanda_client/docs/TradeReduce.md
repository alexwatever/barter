# TradeReduce

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**trade_id** | Option<**String**> | The ID of the Trade that was reduced or closed | [optional]
**units** | Option<**String**> | The number of units that the Trade was reduced by | [optional]
**price** | Option<**String**> | The average price that the units were closed at. This price may be clamped for guaranteed Stop Loss Orders. | [optional]
**realized_pl** | Option<**String**> | The PL realized when reducing the Trade | [optional]
**financing** | Option<**String**> | The financing paid/collected when reducing the Trade | [optional]
**guaranteed_execution_fee** | Option<**String**> | This is the fee that is charged for closing the Trade if it has a guaranteed Stop Loss Order attached to it. | [optional]
**half_spread_cost** | Option<**String**> | The half spread cost for the trade reduce/close. This can be a positive or negative value and is represented in the home currency of the Account. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


