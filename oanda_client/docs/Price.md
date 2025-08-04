# Price

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**instrument** | Option<**String**> | The Price's Instrument. | [optional]
**tradeable** | Option<**bool**> | Flag indicating if the Price is tradeable or not | [optional]
**timestamp** | Option<**String**> | The date/time when the Price was created. | [optional]
**base_bid** | Option<**String**> | The base bid price as calculated by pricing. | [optional]
**base_ask** | Option<**String**> | The base ask price as calculated by pricing. | [optional]
**bids** | Option<[**Vec<models::PriceBucket>**](PriceBucket.md)> | The list of prices and liquidity available on the Instrument's bid side. It is possible for this list to be empty if there is no bid liquidity currently available for the Instrument in the Account. | [optional]
**asks** | Option<[**Vec<models::PriceBucket>**](PriceBucket.md)> | The list of prices and liquidity available on the Instrument's ask side. It is possible for this list to be empty if there is no ask liquidity currently available for the Instrument in the Account. | [optional]
**closeout_bid** | Option<**String**> | The closeout bid price. This price is used when a bid is required to closeout a Position (margin closeout or manual) yet there is no bid liquidity. The closeout bid is never used to open a new position. | [optional]
**closeout_ask** | Option<**String**> | The closeout ask price. This price is used when an ask is required to closeout a Position (margin closeout or manual) yet there is no ask liquidity. The closeout ask is never used to open a new position. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


