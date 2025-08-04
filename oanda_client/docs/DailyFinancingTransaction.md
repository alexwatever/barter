# DailyFinancingTransaction

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**String**> | The Transaction's Identifier. | [optional]
**time** | Option<**String**> | The date/time when the Transaction was created. | [optional]
**user_id** | Option<**i32**> | The ID of the user that initiated the creation of the Transaction. | [optional]
**account_id** | Option<**String**> | The ID of the Account the Transaction was created for. | [optional]
**batch_id** | Option<**String**> | The ID of the \"batch\" that the Transaction belongs to. Transactions in the same batch are applied to the Account simultaneously. | [optional]
**request_id** | Option<**String**> | The Request ID of the request which generated the transaction. | [optional]
**r#type** | Option<**String**> | The Type of the Transaction. Always set to \"DAILY_FINANCING\" for a DailyFinancingTransaction. | [optional]
**financing** | Option<**String**> | The amount of financing paid/collected for the Account. | [optional]
**account_balance** | Option<**String**> | The Account's balance after daily financing. | [optional]
**account_financing_mode** | Option<**String**> | The account financing mode at the time of the daily financing. | [optional]
**position_financings** | Option<[**Vec<models::PositionFinancing>**](PositionFinancing.md)> | The financing paid/collected for each Position in the Account. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


