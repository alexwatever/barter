# ListTransactions200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**from** | Option<**String**> | The starting time provided in the request. | [optional]
**to** | Option<**String**> | The ending time provided in the request. | [optional]
**page_size** | Option<**i32**> | The pageSize provided in the request | [optional]
**r#type** | Option<**Vec<String>**> | The Transaction-type filter provided in the request | [optional]
**count** | Option<**i32**> | The number of Transactions that are contained in the pages returned | [optional]
**pages** | Option<**Vec<String>**> | The list of URLs that represent idrange queries providing the data for each page in the query results | [optional]
**last_transaction_id** | Option<**String**> | The ID of the most recent Transaction created for the Account | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


