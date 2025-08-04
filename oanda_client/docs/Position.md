# Position

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**instrument** | Option<**String**> | The Position's Instrument. | [optional]
**pl** | Option<**String**> | Profit/loss realized by the Position over the lifetime of the Account. | [optional]
**unrealized_pl** | Option<**String**> | The unrealized profit/loss of all open Trades that contribute to this Position. | [optional]
**margin_used** | Option<**String**> | Margin currently used by the Position. | [optional]
**resettable_pl** | Option<**String**> | Profit/loss realized by the Position since the Account's resettablePL was last reset by the client. | [optional]
**financing** | Option<**String**> | The total amount of financing paid/collected for this instrument over the lifetime of the Account. | [optional]
**commission** | Option<**String**> | The total amount of commission paid for this instrument over the lifetime of the Account. | [optional]
**guaranteed_execution_fees** | Option<**String**> | The total amount of fees charged over the lifetime of the Account for the execution of guaranteed Stop Loss Orders for this instrument. | [optional]
**long** | Option<[**models::PositionSide**](PositionSide.md)> |  | [optional]
**short** | Option<[**models::PositionSide**](PositionSide.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


