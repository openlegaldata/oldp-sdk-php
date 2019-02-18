# Court

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**name** | **string** | Full name of the court with location | 
**court_type** | **string** | Court type AG,VG,... | [optional] 
**city** | **int** | Court belongs to this city, if null court is state-level | [optional] 
**state** | **int** | Court belongs to this state (derive country of this field) | 
**code** | **string** | Unique court identifier based on ECLI (e.g. BVerfG) | 
**slug** | **string** | Type &amp; city name as lowercase | 
**description** | **string** |  | [optional] 
**image** | **string** |  | [optional] 
**homepage** | **string** | Official court homepage | [optional] 
**street_address** | **string** | Street address with house number | [optional] 
**postal_code** | **string** | Postal code (ZIP code) | [optional] 
**address_locality** | **string** | Locality (city name) | [optional] 
**telephone** | **string** | Telephone number | [optional] 
**fax_number** | **string** | Fax number | [optional] 
**jurisdiction** | **string** | Jurisdiction of court (ordinary, civil, ...) | [optional] 
**level_of_appeal** | **string** | Subject-matter jurisdiction (local, federal, high court, ...) | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


