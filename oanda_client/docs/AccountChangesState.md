# AccountChangesState

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**unrealized_pl** | Option<**String**> | The total unrealized profit/loss for all Trades currently open in the Account. | [optional]
**nav** | Option<**String**> | The net asset value of the Account. Equal to Account balance + unrealizedPL. | [optional]
**margin_used** | Option<**String**> | Margin currently used for the Account. | [optional]
**margin_available** | Option<**String**> | Margin available for Account currency. | [optional]
**position_value** | Option<**String**> | The value of the Account's open positions represented in the Account's home currency. | [optional]
**margin_closeout_unrealized_pl** | Option<**String**> | The Account's margin closeout unrealized PL. | [optional]
**margin_closeout_nav** | Option<**String**> | The Account's margin closeout NAV. | [optional]
**margin_closeout_margin_used** | Option<**String**> | The Account's margin closeout margin used. | [optional]
**margin_closeout_percent** | Option<**String**> | The Account's margin closeout percentage. When this value is 1.0 or above the Account is in a margin closeout situation. | [optional]
**margin_closeout_position_value** | Option<**String**> | The value of the Account's open positions as used for margin closeout calculations represented in the Account's home currency. | [optional]
**withdrawal_limit** | Option<**String**> | The current WithdrawalLimit for the account which will be zero or a positive value indicating how much can be withdrawn from the account. | [optional]
**margin_call_margin_used** | Option<**String**> | The Account's margin call margin used. | [optional]
**margin_call_percent** | Option<**String**> | The Account's margin call percentage. When this value is 1.0 or above the Account is in a margin call situation. | [optional]
**orders** | Option<[**Vec<models::DynamicOrderState>**](DynamicOrderState.md)> | The price-dependent state of each pending Order in the Account. | [optional]
**trades** | Option<[**Vec<models::CalculatedTradeState>**](CalculatedTradeState.md)> | The price-dependent state for each open Trade in the Account. | [optional]
**positions** | Option<[**Vec<models::CalculatedPositionState>**](CalculatedPositionState.md)> | The price-dependent state for each open Position in the Account. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


