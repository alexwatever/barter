# CreateTransaction

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**String**> | The Transaction's Identifier. | [optional]
**time** | Option<**String**> | The date/time when the Transaction was created. | [optional]
**user_id** | Option<**i32**> | The ID of the user that initiated the creation of the Transaction. | [optional]
**account_id** | Option<**String**> | The ID of the Account the Transaction was created for. | [optional]
**batch_id** | Option<**String**> | The ID of the \"batch\" that the Transaction belongs to. Transactions in the same batch are applied to the Account simultaneously. | [optional]
**request_id** | Option<**String**> | The Request ID of the request which generated the transaction. | [optional]
**r#type** | Option<**String**> | The Type of the Transaction. Always set to \"CREATE\" in a CreateTransaction. | [optional]
**division_id** | Option<**i32**> | The ID of the Division that the Account is in | [optional]
**site_id** | Option<**i32**> | The ID of the Site that the Account was created at | [optional]
**account_user_id** | Option<**i32**> | The ID of the user that the Account was created for | [optional]
**account_number** | Option<**i32**> | The number of the Account within the site/division/user | [optional]
**home_currency** | Option<**String**> | The home currency of the Account | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


