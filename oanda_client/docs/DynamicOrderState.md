# DynamicOrderState

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**String**> | The Order's ID. | [optional]
**trailing_stop_value** | Option<**String**> | The Order's calculated trailing stop value. | [optional]
**trigger_distance** | Option<**String**> | The distance between the Trailing Stop Loss Order's trailingStopValue and the current Market Price. This represents the distance (in price units) of the Order from a triggering price. If the distance could not be determined, this value will not be set. | [optional]
**is_trigger_distance_exact** | Option<**bool**> | True if an exact trigger distance could be calculated. If false, it means the provided trigger distance is a best estimate. If the distance could not be determined, this value will not be set. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


