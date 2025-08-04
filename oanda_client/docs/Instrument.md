# Instrument

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | Option<**String**> | The name of the Instrument | [optional]
**r#type** | Option<**String**> | The type of the Instrument | [optional]
**display_name** | Option<**String**> | The display name of the Instrument | [optional]
**pip_location** | Option<**i32**> | The location of the \"pip\" for this instrument. The decimal position of the pip in this Instrument's price can be found at 10 ^ pipLocation (e.g. -4 pipLocation results in a decimal pip position of 10 ^ -4 = 0.0001). | [optional]
**display_precision** | Option<**i32**> | The number of decimal places that should be used to display prices for this instrument. (e.g. a displayPrecision of 5 would result in a price of \"1\" being displayed as \"1.00000\") | [optional]
**trade_units_precision** | Option<**i32**> | The amount of decimal places that may be provided when specifying the number of units traded for this instrument. | [optional]
**minimum_trade_size** | Option<**String**> | The smallest number of units allowed to be traded for this instrument. | [optional]
**maximum_trailing_stop_distance** | Option<**String**> | The maximum trailing stop distance allowed for a trailing stop loss created for this instrument. Specified in price units. | [optional]
**minimum_trailing_stop_distance** | Option<**String**> | The minimum trailing stop distance allowed for a trailing stop loss created for this instrument. Specified in price units. | [optional]
**maximum_position_size** | Option<**String**> | The maximum position size allowed for this instrument. Specified in units. | [optional]
**maximum_order_units** | Option<**String**> | The maximum units allowed for an Order placed for this instrument. Specified in units. | [optional]
**margin_rate** | Option<**String**> | The margin rate for this instrument. | [optional]
**commission** | Option<[**models::InstrumentCommission**](InstrumentCommission.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


