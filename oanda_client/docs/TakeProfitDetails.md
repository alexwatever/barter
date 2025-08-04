# TakeProfitDetails

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**price** | Option<**String**> | The price that the Take Profit Order will be triggered at. Only one of the price and distance fields may be specified. | [optional]
**time_in_force** | Option<**String**> | The time in force for the created Take Profit Order. This may only be GTC, GTD or GFD. | [optional]
**gtd_time** | Option<**String**> | The date when the Take Profit Order will be cancelled on if timeInForce is GTD. | [optional]
**client_extensions** | Option<[**models::ClientExtensions**](ClientExtensions.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


