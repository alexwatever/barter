# HomeConversions

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currency** | Option<**String**> | The currency to be converted into the home currency. | [optional]
**account_gain** | Option<**String**> | The factor used to convert any gains for an Account in the specified currency into the Account's home currency. This would include positive realized P/L and positive financing amounts. Conversion is performed by multiplying the positive P/L by the conversion factor. | [optional]
**account_loss** | Option<**String**> | The string representation of a decimal number. | [optional]
**position_value** | Option<**String**> | The factor used to convert a Position or Trade Value in the specified currency into the Account's home currency. Conversion is performed by multiplying the Position or Trade Value by the conversion factor. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


