# GetPrices200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**prices** | Option<[**Vec<models::ClientPrice>**](ClientPrice.md)> | The list of Price objects requested. | [optional]
**home_conversions** | Option<[**Vec<models::HomeConversions>**](HomeConversions.md)> | The list of home currency conversion factors requested. This field will only be present if includeHomeConversions was set to true in the request. | [optional]
**time** | Option<**String**> | The DateTime value to use for the \"since\" parameter in the next poll request. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


