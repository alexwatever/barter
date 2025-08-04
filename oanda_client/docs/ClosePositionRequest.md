# ClosePositionRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**long_units** | Option<**String**> | Indication of how much of the long Position to closeout. Either the string \"ALL\", the string \"NONE\", or a DecimalNumber representing how many units of the long position to close using a PositionCloseout MarketOrder. The units specified must always be positive. | [optional]
**long_client_extensions** | Option<[**models::ClientExtensions**](ClientExtensions.md)> |  | [optional]
**short_units** | Option<**String**> | Indication of how much of the short Position to closeout. Either the string \"ALL\", the string \"NONE\", or a DecimalNumber representing how many units of the short position to close using a PositionCloseout MarketOrder. The units specified must always be positive. | [optional]
**short_client_extensions** | Option<[**models::ClientExtensions**](ClientExtensions.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


