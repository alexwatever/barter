# PositionBook

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**instrument** | Option<**String**> | The position book's instrument | [optional]
**time** | Option<**String**> | The time when the position book snapshot was created | [optional]
**price** | Option<**String**> | The price (midpoint) for the position book's instrument at the time of the position book snapshot | [optional]
**bucket_width** | Option<**String**> | The price width for each bucket. Each bucket covers the price range from the bucket's price to the bucket's price + bucketWidth. | [optional]
**buckets** | Option<[**Vec<models::PositionBookBucket>**](PositionBookBucket.md)> | The partitioned position book, divided into buckets using a default bucket width. These buckets are only provided for price ranges which actually contain order or position data. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


