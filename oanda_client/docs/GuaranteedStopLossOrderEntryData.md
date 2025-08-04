# GuaranteedStopLossOrderEntryData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**minimum_distance** | Option<**String**> | The minimum distance allowed between the Trade's fill price and the configured price for guaranteed Stop Loss Orders created for this instrument. Specified in price units. | [optional]
**premium** | Option<**String**> | The amount that is charged to the account if a guaranteed Stop Loss Order is triggered and filled. The value is in price units and is charged for each unit of the Trade. | [optional]
**level_restriction** | Option<[**models::GuaranteedStopLossOrderLevelRestriction**](GuaranteedStopLossOrderLevelRestriction.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


