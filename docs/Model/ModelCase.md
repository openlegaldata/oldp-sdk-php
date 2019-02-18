# ModelCase

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**slug** | **string** |  | [optional] 
**court** | [**\Swagger\Client\Model\CourtMinimal**](CourtMinimal.md) |  | [optional] 
**file_number** | **string** | File number as defined by court | 
**date** | [**\DateTime**](\DateTime.md) | Publication date as in source | [optional] 
**created_date** | [**\DateTime**](\DateTime.md) | Entry is created at this date time | [optional] 
**updated_date** | [**\DateTime**](\DateTime.md) | Date time of last change | [optional] 
**type** | **string** | Type of decision (Urteil, Beschluss, ...) | [optional] 
**ecli** | **string** | European Case Law Identifier | [optional] 
**content** | **string** | Case full-text formatted in Legal HTML | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


