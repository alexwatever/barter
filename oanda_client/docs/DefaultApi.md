# \DefaultApi

All URIs are relative to */v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancel_order**](DefaultApi.md#cancel_order) | **PUT** /accounts/{accountID}/orders/{orderSpecifier}/cancel | Cancel Order
[**close_position**](DefaultApi.md#close_position) | **PUT** /accounts/{accountID}/positions/{instrument}/close | Close Position
[**close_trade**](DefaultApi.md#close_trade) | **PUT** /accounts/{accountID}/trades/{tradeSpecifier}/close | Close Trade
[**configure_account**](DefaultApi.md#configure_account) | **PATCH** /accounts/{accountID}/configuration | Configure Account
[**create_order**](DefaultApi.md#create_order) | **POST** /accounts/{accountID}/orders | Create Order
[**get_account**](DefaultApi.md#get_account) | **GET** /accounts/{accountID} | Account Details
[**get_account_changes**](DefaultApi.md#get_account_changes) | **GET** /accounts/{accountID}/changes | Poll Account Updates
[**get_account_instrument_candles**](DefaultApi.md#get_account_instrument_candles) | **GET** /accounts/{accountID}/instruments/{instrument}/candles | Get Candlesticks
[**get_account_instruments**](DefaultApi.md#get_account_instruments) | **GET** /accounts/{accountID}/instruments | Account Instruments
[**get_account_summary**](DefaultApi.md#get_account_summary) | **GET** /accounts/{accountID}/summary | Account Summary
[**get_base_prices**](DefaultApi.md#get_base_prices) | **GET** /pricing | Get Base Prices
[**get_external_user_info**](DefaultApi.md#get_external_user_info) | **GET** /users/{userSpecifier}/externalInfo | External User Info
[**get_instrument_candles**](DefaultApi.md#get_instrument_candles) | **GET** /instruments/{instrument}/candles | Get Candlesticks
[**get_instrument_price**](DefaultApi.md#get_instrument_price) | **GET** /instruments/{instrument}/price | Price
[**get_instrument_price_range**](DefaultApi.md#get_instrument_price_range) | **GET** /instruments/{instrument}/price/range | Get Prices
[**get_order**](DefaultApi.md#get_order) | **GET** /accounts/{accountID}/orders/{orderSpecifier} | Get Order
[**get_position**](DefaultApi.md#get_position) | **GET** /accounts/{accountID}/positions/{instrument} | Instrument Position
[**get_price_range**](DefaultApi.md#get_price_range) | **GET** /pricing/range | Get Price Range
[**get_prices**](DefaultApi.md#get_prices) | **GET** /accounts/{accountID}/pricing | Current Account Prices
[**get_trade**](DefaultApi.md#get_trade) | **GET** /accounts/{accountID}/trades/{tradeSpecifier} | Trade Details
[**get_transaction**](DefaultApi.md#get_transaction) | **GET** /accounts/{accountID}/transactions/{transactionID} | Transaction Details
[**get_transaction_range**](DefaultApi.md#get_transaction_range) | **GET** /accounts/{accountID}/transactions/idrange | Transaction ID Range
[**get_transactions_since_id**](DefaultApi.md#get_transactions_since_id) | **GET** /accounts/{accountID}/transactions/sinceid | Transactions Since ID
[**get_user_info**](DefaultApi.md#get_user_info) | **GET** /users/{userSpecifier} | User Info
[**instruments_instrument_order_book_get**](DefaultApi.md#instruments_instrument_order_book_get) | **GET** /instruments/{instrument}/orderBook | Get Order Book
[**instruments_instrument_position_book_get**](DefaultApi.md#instruments_instrument_position_book_get) | **GET** /instruments/{instrument}/positionBook | Get Position Book
[**list_accounts**](DefaultApi.md#list_accounts) | **GET** /accounts | List Accounts
[**list_open_positions**](DefaultApi.md#list_open_positions) | **GET** /accounts/{accountID}/openPositions | Open Positions
[**list_open_trades**](DefaultApi.md#list_open_trades) | **GET** /accounts/{accountID}/openTrades | List Open Trades
[**list_orders**](DefaultApi.md#list_orders) | **GET** /accounts/{accountID}/orders | List Orders
[**list_pending_orders**](DefaultApi.md#list_pending_orders) | **GET** /accounts/{accountID}/pendingOrders | Pending Orders
[**list_positions**](DefaultApi.md#list_positions) | **GET** /accounts/{accountID}/positions | List Positions
[**list_trades**](DefaultApi.md#list_trades) | **GET** /accounts/{accountID}/trades | List Trades
[**list_transactions**](DefaultApi.md#list_transactions) | **GET** /accounts/{accountID}/transactions | List Transactions
[**replace_order**](DefaultApi.md#replace_order) | **PUT** /accounts/{accountID}/orders/{orderSpecifier} | Replace Order
[**set_order_client_extensions**](DefaultApi.md#set_order_client_extensions) | **PUT** /accounts/{accountID}/orders/{orderSpecifier}/clientExtensions | Set Order Extensions
[**set_trade_client_extensions**](DefaultApi.md#set_trade_client_extensions) | **PUT** /accounts/{accountID}/trades/{tradeSpecifier}/clientExtensions | Set Trade Client Extensions
[**set_trade_dependent_orders**](DefaultApi.md#set_trade_dependent_orders) | **PUT** /accounts/{accountID}/trades/{tradeSpecifier}/orders | Set Dependent Orders
[**stream_pricing**](DefaultApi.md#stream_pricing) | **GET** /accounts/{accountID}/pricing/stream | Price Stream
[**stream_transactions**](DefaultApi.md#stream_transactions) | **GET** /accounts/{accountID}/transactions/stream | Transaction Stream



## cancel_order

> models::CancelOrder200Response cancel_order(authorization, account_id, order_specifier, accept_datetime_format, client_request_id)
Cancel Order

Cancel a pending Order in an Account

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**order_specifier** | **String** | The Order Specifier | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |
**client_request_id** | Option<**String**> | Client specified RequestID to be sent with request. |  |

### Return type

[**models::CancelOrder200Response**](cancelOrder_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## close_position

> models::ClosePosition200Response close_position(authorization, account_id, instrument, close_position_body, accept_datetime_format)
Close Position

Closeout the open Position for a specific instrument in an Account.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**instrument** | **String** | Name of the Instrument | [required] |
**close_position_body** | [**ClosePositionRequest**](ClosePositionRequest.md) | Representation of how to close the position | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |

### Return type

[**models::ClosePosition200Response**](closePosition_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## close_trade

> models::CloseTrade200Response close_trade(authorization, account_id, trade_specifier, close_trade_body, accept_datetime_format)
Close Trade

Close (partially or fully) a specific open Trade in an Account

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**trade_specifier** | **String** | Specifier for the Trade | [required] |
**close_trade_body** | [**CloseTradeRequest**](CloseTradeRequest.md) | Details of how much of the open Trade to close. | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |

### Return type

[**models::CloseTrade200Response**](closeTrade_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## configure_account

> models::ConfigureAccount200Response configure_account(authorization, account_id, accept_datetime_format, configure_account_body)
Configure Account

Set the client-configurable portions of an Account.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |
**configure_account_body** | Option<[**ConfigureAccountRequest**](ConfigureAccountRequest.md)> | Representation of the Account configuration to set |  |

### Return type

[**models::ConfigureAccount200Response**](configureAccount_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_order

> models::CreateOrder201Response create_order(authorization, account_id, create_order_body, accept_datetime_format)
Create Order

Create an Order for an Account

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**create_order_body** | [**CreateOrderRequest**](CreateOrderRequest.md) |  | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |

### Return type

[**models::CreateOrder201Response**](createOrder_201_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_account

> models::GetAccount200Response get_account(authorization, account_id, accept_datetime_format)
Account Details

Get the full details for a single Account that a client has access to. Full pending Order, open Trade and open Position representations are provided.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |

### Return type

[**models::GetAccount200Response**](getAccount_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_account_changes

> models::GetAccountChanges200Response get_account_changes(authorization, account_id, accept_datetime_format, since_transaction_id)
Poll Account Updates

Endpoint used to poll an Account for its current state and changes since a specified TransactionID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |
**since_transaction_id** | Option<**String**> | ID of the Transaction to get Account changes since. |  |

### Return type

[**models::GetAccountChanges200Response**](getAccountChanges_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_account_instrument_candles

> models::GetInstrumentCandles200Response get_account_instrument_candles(authorization, instrument, accept_datetime_format, price, granularity, count, from, to, smooth, include_first, daily_alignment, alignment_timezone, weekly_alignment, units)
Get Candlesticks

Fetch candlestick data for an instrument.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**instrument** | **String** | Name of the Instrument | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |
**price** | Option<**String**> | The Price component(s) to get candlestick data for. Can contain any combination of the characters \"M\" (midpoint candles) \"B\" (bid candles) and \"A\" (ask candles). |  |
**granularity** | Option<**String**> | The granularity of the candlesticks to fetch |  |
**count** | Option<**i32**> | The number of candlesticks to return in the response. Count should not be specified if both the start and end parameters are provided, as the time range combined with the granularity will determine the number of candlesticks to return. |  |
**from** | Option<**String**> | The start of the time range to fetch candlesticks for. |  |
**to** | Option<**String**> | The end of the time range to fetch candlesticks for. |  |
**smooth** | Option<**bool**> | A flag that controls whether the candlestick is \"smoothed\" or not.  A smoothed candlestick uses the previous candle's close price as its open price, while an unsmoothed candlestick uses the first price from its time range as its open price. |  |
**include_first** | Option<**bool**> | A flag that controls whether the candlestick that is covered by the from time should be included in the results. This flag enables clients to use the timestamp of the last completed candlestick received to poll for future candlesticks but avoid receiving the previous candlestick repeatedly. |  |
**daily_alignment** | Option<**i32**> | The hour of the day (in the specified timezone) to use for granularities that have daily alignments. |  |
**alignment_timezone** | Option<**String**> | The timezone to use for the dailyAlignment parameter. Candlesticks with daily alignment will be aligned to the dailyAlignment hour within the alignmentTimezone.  Note that the returned times will still be represented in UTC. |  |
**weekly_alignment** | Option<**String**> | The day of the week used for granularities that have weekly alignment. |  |
**units** | Option<**String**> | The number of units used to calculate the volume-weighted average bid and ask prices in the returned candles. |  |

### Return type

[**models::GetInstrumentCandles200Response**](getInstrumentCandles_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_account_instruments

> models::GetAccountInstruments200Response get_account_instruments(authorization, account_id, instruments)
Account Instruments

Get the list of tradeable instruments for the given Account. The list of tradeable instruments is dependent on the regulatory division that the Account is located in, thus should be the same for all Accounts owned by a single user.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**instruments** | Option<[**Vec<String>**](String.md)> | List of instruments to query specifically. |  |

### Return type

[**models::GetAccountInstruments200Response**](getAccountInstruments_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_account_summary

> models::GetAccountSummary200Response get_account_summary(authorization, account_id, accept_datetime_format)
Account Summary

Get a summary for a single Account that a client has access to.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |

### Return type

[**models::GetAccountSummary200Response**](getAccountSummary_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_base_prices

> models::GetInstrumentPriceRange200Response get_base_prices(authorization, accept_datetime_format, time)
Get Base Prices

Get pricing information for a specified instrument. Accounts are not associated in any way with this endpoint.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |
**time** | Option<**String**> | The time at which the desired price for each instrument is in effect. The current price for each instrument is returned if no time is provided. |  |

### Return type

[**models::GetInstrumentPriceRange200Response**](getInstrumentPriceRange_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_external_user_info

> models::GetExternalUserInfo200Response get_external_user_info(authorization, user_specifier)
External User Info

Fetch the externally-available user information for the specified user. This endpoint is intended to be used by 3rd parties that have been authorized by a user to view their personal information.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**user_specifier** | **String** | The User Specifier | [required] |

### Return type

[**models::GetExternalUserInfo200Response**](getExternalUserInfo_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_instrument_candles

> models::GetInstrumentCandles200Response get_instrument_candles(authorization, instrument, accept_datetime_format, price, granularity, count, from, to, smooth, include_first, daily_alignment, alignment_timezone, weekly_alignment)
Get Candlesticks

Fetch candlestick data for an instrument.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**instrument** | **String** | Name of the Instrument | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |
**price** | Option<**String**> | The Price component(s) to get candlestick data for. Can contain any combination of the characters \"M\" (midpoint candles) \"B\" (bid candles) and \"A\" (ask candles). |  |
**granularity** | Option<**String**> | The granularity of the candlesticks to fetch |  |
**count** | Option<**i32**> | The number of candlesticks to return in the reponse. Count should not be specified if both the start and end parameters are provided, as the time range combined with the graularity will determine the number of candlesticks to return. |  |
**from** | Option<**String**> | The start of the time range to fetch candlesticks for. |  |
**to** | Option<**String**> | The end of the time range to fetch candlesticks for. |  |
**smooth** | Option<**bool**> | A flag that controls whether the candlestick is \"smoothed\" or not.  A smoothed candlestick uses the previous candle's close price as its open price, while an unsmoothed candlestick uses the first price from its time range as its open price. |  |
**include_first** | Option<**bool**> | A flag that controls whether the candlestick that is covered by the from time should be included in the results. This flag enables clients to use the timestamp of the last completed candlestick received to poll for future candlesticks but avoid receiving the previous candlestick repeatedly. |  |
**daily_alignment** | Option<**i32**> | The hour of the day (in the specified timezone) to use for granularities that have daily alignments. |  |
**alignment_timezone** | Option<**String**> | The timezone to use for the dailyAlignment parameter. Candlesticks with daily alignment will be aligned to the dailyAlignment hour within the alignmentTimezone.  Note that the returned times will still be represented in UTC. |  |
**weekly_alignment** | Option<**String**> | The day of the week used for granularities that have weekly alignment. |  |

### Return type

[**models::GetInstrumentCandles200Response**](getInstrumentCandles_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_instrument_price

> models::GetInstrumentPrice200Response get_instrument_price(authorization, instrument, accept_datetime_format, time)
Price

Fetch a price for an instrument. Accounts are not associated in any way with this endpoint.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**instrument** | **String** | Name of the Instrument | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |
**time** | Option<**String**> | The time at which the desired price is in effect. The current price is returned if no time is provided. |  |

### Return type

[**models::GetInstrumentPrice200Response**](getInstrumentPrice_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_instrument_price_range

> models::GetInstrumentPriceRange200Response get_instrument_price_range(authorization, instrument, from, accept_datetime_format, to)
Get Prices

Fetch a range of prices for an instrument. Accounts are not associated in any way with this endpoint.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**instrument** | **String** | Name of the Instrument | [required] |
**from** | **String** | The start of the time range to fetch prices for. | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |
**to** | Option<**String**> | The end of the time range to fetch prices for. The current time is used if this parameter is not provided. |  |

### Return type

[**models::GetInstrumentPriceRange200Response**](getInstrumentPriceRange_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_order

> models::GetOrder200Response get_order(authorization, account_id, order_specifier, accept_datetime_format)
Get Order

Get details for a single Order in an Account

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**order_specifier** | **String** | The Order Specifier | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |

### Return type

[**models::GetOrder200Response**](getOrder_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_position

> models::GetPosition200Response get_position(authorization, account_id, instrument)
Instrument Position

Get the details of a single Instrument's Position in an Account. The Position may by open or not.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**instrument** | **String** | Name of the Instrument | [required] |

### Return type

[**models::GetPosition200Response**](getPosition_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_price_range

> models::GetInstrumentPriceRange200Response get_price_range(authorization, instrument, from, accept_datetime_format, to)
Get Price Range

Get pricing information for a specified range of prices. Accounts are not associated in any way with this endpoint.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**instrument** | **String** | Name of the Instrument | [required] |
**from** | **String** | The start of the time range to fetch prices for. | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |
**to** | Option<**String**> | The end of the time range to fetch prices for. The current time is used if this parameter is not provided. |  |

### Return type

[**models::GetInstrumentPriceRange200Response**](getInstrumentPriceRange_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_prices

> models::GetPrices200Response get_prices(authorization, account_id, instruments, accept_datetime_format, since, include_units_available, include_home_conversions)
Current Account Prices

Get pricing information for a specified list of Instruments within an Account.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**instruments** | [**Vec<String>**](String.md) | List of Instruments to get pricing for. | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |
**since** | Option<**String**> | Date/Time filter to apply to the response. Only prices and home conversions (if requested) with a time later than this filter (i.e. the price has changed after the since time) will be provided, and are filtered independently. |  |
**include_units_available** | Option<**bool**> | Flag that enables the inclusion of the unitsAvailable field in the returned Price objects. |  |
**include_home_conversions** | Option<**bool**> | Flag that enables the inclusion of the homeConversions field in the returned response. An entry will be returned for each currency in the set of all base and quote currencies present in the requested instruments list. |  |

### Return type

[**models::GetPrices200Response**](getPrices_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_trade

> models::GetTrade200Response get_trade(authorization, account_id, trade_specifier, accept_datetime_format)
Trade Details

Get the details of a specific Trade in an Account

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**trade_specifier** | **String** | Specifier for the Trade | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |

### Return type

[**models::GetTrade200Response**](getTrade_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_transaction

> models::GetTransaction200Response get_transaction(authorization, account_id, transaction_id, accept_datetime_format)
Transaction Details

Get the details of a single Account Transaction.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**transaction_id** | **String** | A Transaction ID | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |

### Return type

[**models::GetTransaction200Response**](getTransaction_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_transaction_range

> models::GetTransactionRange200Response get_transaction_range(authorization, account_id, from, to, accept_datetime_format, r#type)
Transaction ID Range

Get a range of Transactions for an Account based on the Transaction IDs.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**from** | **String** | The starting Transacion ID (inclusive) to fetch. | [required] |
**to** | **String** | The ending Transaction ID (inclusive) to fetch. | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |
**r#type** | Option<[**Vec<String>**](String.md)> | The filter that restricts the types of Transactions to retreive. |  |

### Return type

[**models::GetTransactionRange200Response**](getTransactionRange_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_transactions_since_id

> models::GetTransactionRange200Response get_transactions_since_id(authorization, account_id, id, accept_datetime_format)
Transactions Since ID

Get a range of Transactions for an Account starting at (but not including) a provided Transaction ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**id** | **String** | The ID of the last Transacion fetched. This query will return all Transactions newer than the TransactionID. | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |

### Return type

[**models::GetTransactionRange200Response**](getTransactionRange_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_user_info

> models::GetUserInfo200Response get_user_info(authorization, user_specifier)
User Info

Fetch the user information for the specified user. This endpoint is intended to be used by the user themself to obtain their own information.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**user_specifier** | **String** | The User Specifier | [required] |

### Return type

[**models::GetUserInfo200Response**](getUserInfo_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## instruments_instrument_order_book_get

> models::InstrumentsInstrumentOrderBookGet200Response instruments_instrument_order_book_get(authorization, instrument, accept_datetime_format, time)
Get Order Book

Fetch an order book for an instrument.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**instrument** | **String** | Name of the Instrument | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |
**time** | Option<**String**> | The time of the snapshot to fetch. If not specified, then the most recent snapshot is fetched. |  |

### Return type

[**models::InstrumentsInstrumentOrderBookGet200Response**](_instruments__instrument__orderBook_get_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## instruments_instrument_position_book_get

> models::InstrumentsInstrumentPositionBookGet200Response instruments_instrument_position_book_get(authorization, instrument, accept_datetime_format, time)
Get Position Book

Fetch a position book for an instrument.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**instrument** | **String** | Name of the Instrument | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |
**time** | Option<**String**> | The time of the snapshot to fetch. If not specified, then the most recent snapshot is fetched. |  |

### Return type

[**models::InstrumentsInstrumentPositionBookGet200Response**](_instruments__instrument__positionBook_get_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## list_accounts

> models::ListAccounts200Response list_accounts(authorization)
List Accounts

Get a list of all Accounts authorized for the provided token.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |

### Return type

[**models::ListAccounts200Response**](listAccounts_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## list_open_positions

> models::ListOpenPositions200Response list_open_positions(authorization, account_id)
Open Positions

List all open Positions for an Account. An open Position is a Position in an Account that currently has a Trade opened for it.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |

### Return type

[**models::ListOpenPositions200Response**](listOpenPositions_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## list_open_trades

> models::ListOpenTrades200Response list_open_trades(authorization, account_id, accept_datetime_format)
List Open Trades

Get the list of open Trades for an Account

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |

### Return type

[**models::ListOpenTrades200Response**](listOpenTrades_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## list_orders

> models::ListOrders200Response list_orders(authorization, account_id, accept_datetime_format, ids, state, instrument, count, before_id)
List Orders

Get a list of Orders for an Account

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |
**ids** | Option<[**Vec<String>**](String.md)> | List of Order IDs to retrieve |  |
**state** | Option<**String**> | The state to filter the requested Orders by |  |
**instrument** | Option<**String**> | The instrument to filter the requested orders by |  |
**count** | Option<**i32**> | The maximum number of Orders to return |  |
**before_id** | Option<**String**> | The maximum Order ID to return. If not provided the most recent Orders in the Account are returned |  |

### Return type

[**models::ListOrders200Response**](listOrders_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## list_pending_orders

> models::ListPendingOrders200Response list_pending_orders(authorization, account_id, accept_datetime_format)
Pending Orders

List all pending Orders in an Account

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |

### Return type

[**models::ListPendingOrders200Response**](listPendingOrders_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## list_positions

> models::ListPositions200Response list_positions(authorization, account_id)
List Positions

List all Positions for an Account. The Positions returned are for every instrument that has had a position during the lifetime of an the Account.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |

### Return type

[**models::ListPositions200Response**](listPositions_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## list_trades

> models::ListTrades200Response list_trades(authorization, account_id, accept_datetime_format, ids, state, instrument, count, before_id)
List Trades

Get a list of Trades for an Account

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |
**ids** | Option<[**Vec<String>**](String.md)> | List of Trade IDs to retrieve. |  |
**state** | Option<**String**> | The state to filter the requested Trades by. |  |
**instrument** | Option<**String**> | The instrument to filter the requested Trades by. |  |
**count** | Option<**i32**> | The maximum number of Trades to return. |  |
**before_id** | Option<**String**> | The maximum Trade ID to return. If not provided the most recent Trades in the Account are returned. |  |

### Return type

[**models::ListTrades200Response**](listTrades_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## list_transactions

> models::ListTransactions200Response list_transactions(authorization, account_id, accept_datetime_format, from, to, page_size, r#type)
List Transactions

Get a list of Transactions pages that satisfy a time-based Transaction query.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |
**from** | Option<**String**> | The starting time (inclusive) of the time range for the Transactions being queried. |  |
**to** | Option<**String**> | The ending time (inclusive) of the time range for the Transactions being queried. |  |
**page_size** | Option<**i32**> | The number of Transactions to include in each page of the results. |  |
**r#type** | Option<[**Vec<String>**](String.md)> | A filter for restricting the types of Transactions to retreive. |  |

### Return type

[**models::ListTransactions200Response**](listTransactions_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## replace_order

> models::ReplaceOrder201Response replace_order(authorization, account_id, order_specifier, replace_order_body, accept_datetime_format, client_request_id)
Replace Order

Replace an Order in an Account by simultaneously cancelling it and creating a replacement Order

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**order_specifier** | **String** | The Order Specifier | [required] |
**replace_order_body** | [**CreateOrderRequest**](CreateOrderRequest.md) | Specification of the replacing Order. The replacing order must have the same type as the replaced Order. | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |
**client_request_id** | Option<**String**> | Client specified RequestID to be sent with request. |  |

### Return type

[**models::ReplaceOrder201Response**](replaceOrder_201_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## set_order_client_extensions

> models::SetOrderClientExtensions200Response set_order_client_extensions(authorization, account_id, order_specifier, set_order_client_extensions_body, accept_datetime_format)
Set Order Extensions

Update the Client Extensions for an Order in an Account. Do not set, modify, or delete clientExtensions if your account is associated with MT4.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**order_specifier** | **String** | The Order Specifier | [required] |
**set_order_client_extensions_body** | [**SetOrderClientExtensionsRequest**](SetOrderClientExtensionsRequest.md) | Representation of the replacing Order | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |

### Return type

[**models::SetOrderClientExtensions200Response**](setOrderClientExtensions_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## set_trade_client_extensions

> models::SetTradeClientExtensions200Response set_trade_client_extensions(authorization, account_id, trade_specifier, set_trade_client_extensions_body, accept_datetime_format)
Set Trade Client Extensions

Update the Client Extensions for a Trade. Do not add, update, or delete the Client Extensions if your account is associated with MT4.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**trade_specifier** | **String** | Specifier for the Trade | [required] |
**set_trade_client_extensions_body** | [**SetTradeClientExtensionsRequest**](SetTradeClientExtensionsRequest.md) | Details of how to modify the Trade's Client Extensions. | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |

### Return type

[**models::SetTradeClientExtensions200Response**](setTradeClientExtensions_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## set_trade_dependent_orders

> models::SetTradeDependentOrders200Response set_trade_dependent_orders(authorization, account_id, trade_specifier, set_trade_dependent_orders_body, accept_datetime_format)
Set Dependent Orders

Create, replace and cancel a Trade's dependent Orders (Take Profit, Stop Loss and Trailing Stop Loss) through the Trade itself

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**trade_specifier** | **String** | Specifier for the Trade | [required] |
**set_trade_dependent_orders_body** | [**SetTradeDependentOrdersRequest**](SetTradeDependentOrdersRequest.md) | Details of how to modify the Trade's dependent Orders. | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |

### Return type

[**models::SetTradeDependentOrders200Response**](setTradeDependentOrders_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## stream_pricing

> models::StreamPricing200Response stream_pricing(authorization, account_id, instruments, accept_datetime_format, snapshot)
Price Stream

Get a stream of Account Prices starting from when the request is made. This pricing stream does not include every single price created for the Account, but instead will provide at most 4 prices per second (every 250 milliseconds) for each instrument being requested. If more than one price is created for an instrument during the 250 millisecond window, only the price in effect at the end of the window is sent. This means that during periods of rapid price movement, subscribers to this stream will not be sent every price. Pricing windows for different connections to the price stream are not all aligned in the same way (i.e. they are not all aligned to the top of the second). This means that during periods of rapid price movement, different subscribers may observe different prices depending on their alignment.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |
**instruments** | [**Vec<String>**](String.md) | List of Instruments to stream Prices for. | [required] |
**accept_datetime_format** | Option<**String**> | Format of DateTime fields in the request and response. |  |
**snapshot** | Option<**bool**> | Flag that enables/disables the sending of a pricing snapshot when initially connecting to the stream. |  |

### Return type

[**models::StreamPricing200Response**](streamPricing_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## stream_transactions

> models::StreamTransactions200Response stream_transactions(authorization, account_id)
Transaction Stream

Get a stream of Transactions for an Account starting from when the request is made.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**authorization** | **String** | The authorization bearer token previously obtained by the client | [required] |
**account_id** | **String** | Account Identifier | [required] |

### Return type

[**models::StreamTransactions200Response**](streamTransactions_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

