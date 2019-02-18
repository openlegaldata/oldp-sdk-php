# CourtMinimal

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**name** | **string** | Full name of the court with location | 
**slug** | **string** | Type &amp; city name as lowercase | 
**city** | **int** | Court belongs to this city, if null court is state-level | [optional] 
**state** | **int** | Court belongs to this state (derive country of this field) | 
**jurisdiction** | **string** | Jurisdiction of court (ordinary, civil, ...) | [optional] 
**level_of_appeal** | **string** | Subject-matter jurisdiction (local, federal, high court, ...) | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


