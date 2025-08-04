# Candlestick

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**time** | Option<**String**> | The start time of the candlestick | [optional]
**bid** | Option<[**models::CandlestickData**](CandlestickData.md)> |  | [optional]
**ask** | Option<[**models::CandlestickData**](CandlestickData.md)> |  | [optional]
**mid** | Option<[**models::CandlestickData**](CandlestickData.md)> |  | [optional]
**volume** | Option<**i32**> | The number of prices created during the time-range represented by the candlestick. | [optional]
**complete** | Option<**bool**> | A flag indicating if the candlestick is complete. A complete candlestick is one whose ending time is not in the future. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


