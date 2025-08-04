# PositionSide

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**units** | Option<**String**> | Number of units in the position (negative value indicates short position, positive indicates long position). | [optional]
**average_price** | Option<**String**> | Volume-weighted average of the underlying Trade open prices for the Position. | [optional]
**trade_ids** | Option<**Vec<String>**> | List of the open Trade IDs which contribute to the open Position. | [optional]
**pl** | Option<**String**> | Profit/loss realized by the PositionSide over the lifetime of the Account. | [optional]
**unrealized_pl** | Option<**String**> | The unrealized profit/loss of all open Trades that contribute to this PositionSide. | [optional]
**resettable_pl** | Option<**String**> | Profit/loss realized by the PositionSide since the Account's resettablePL was last reset by the client. | [optional]
**financing** | Option<**String**> | The total amount of financing paid/collected for this PositionSide over the lifetime of the Account. | [optional]
**guaranteed_execution_fees** | Option<**String**> | The total amount of fees charged over the lifetime of the Account for the execution of guaranteed Stop Loss Orders attached to Trades for this PositionSide. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


