# AccountSummary

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**String**> | The Account's identifier | [optional]
**alias** | Option<**String**> | Client-assigned alias for the Account. Only provided if the Account has an alias set | [optional]
**currency** | Option<**String**> | The home currency of the Account | [optional]
**balance** | Option<**String**> | The current balance of the Account. | [optional]
**created_by_user_id** | Option<**i32**> | ID of the user that created the Account. | [optional]
**created_time** | Option<**String**> | The date/time when the Account was created. | [optional]
**guaranteed_stop_loss_order_mode** | Option<**String**> | The current guaranteed Stop Loss Order mode of the Account. | [optional]
**pl** | Option<**String**> | The total profit/loss realized over the lifetime of the Account. | [optional]
**resettable_pl** | Option<**String**> | The total realized profit/loss for the Account since it was last reset by the client. | [optional]
**resettable_pl_time** | Option<**String**> | The date/time that the Account's resettablePL was last reset. | [optional]
**financing** | Option<**String**> | The total amount of financing paid/collected over the lifetime of the Account. | [optional]
**commission** | Option<**String**> | The total amount of commission paid over the lifetime of the Account. | [optional]
**guaranteed_execution_fees** | Option<**String**> | The total amount of fees charged over the lifetime of the Account for the execution of guaranteed Stop Loss Orders. | [optional]
**margin_rate** | Option<**String**> | Client-provided margin rate override for the Account. The effective margin rate of the Account is the lesser of this value and the OANDA margin rate for the Account's division. This value is only provided if a margin rate override exists for the Account. | [optional]
**margin_call_enter_time** | Option<**String**> | The date/time when the Account entered a margin call state. Only provided if the Account is in a margin call. | [optional]
**margin_call_extension_count** | Option<**i32**> | The number of times that the Account's current margin call was extended. | [optional]
**last_margin_call_extension_time** | Option<**String**> | The date/time of the Account's last margin call extension. | [optional]
**open_trade_count** | Option<**i32**> | The number of Trades currently open in the Account. | [optional]
**open_position_count** | Option<**i32**> | The number of Positions currently open in the Account. | [optional]
**pending_order_count** | Option<**i32**> | The number of Orders currently pending in the Account. | [optional]
**hedging_enabled** | Option<**bool**> | Flag indicating that the Account has hedging enabled. | [optional]
**last_order_fill_timestamp** | Option<**String**> | The date/time of the last order that was filled for this account. | [optional]
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
**last_transaction_id** | Option<**String**> | The ID of the last Transaction created for the Account. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


