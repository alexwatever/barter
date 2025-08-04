# TrailingStopLossDetails

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**distance** | Option<**String**> | The distance (in price units) from the Trade's fill price that the Trailing Stop Loss Order will be triggered at. | [optional]
**time_in_force** | Option<**String**> | The time in force for the created Trailing Stop Loss Order. This may only be GTC, GTD or GFD. | [optional]
**gtd_time** | Option<**String**> | The date when the Trailing Stop Loss Order will be cancelled on if timeInForce is GTD. | [optional]
**client_extensions** | Option<[**models::ClientExtensions**](ClientExtensions.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


