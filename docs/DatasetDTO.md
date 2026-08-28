# DatasetDTO

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **NullableInt64** |  | [optional] 
**Name** | **string** |  | 
**OwnerTeam** | **string** |  | 
**Tags** | **[]string** |  | 
**Sensitivity** | [**DatasetSensitivity**](DatasetSensitivity.md) |  | 
**SchemaFields** | [**[]FieldDTO**](FieldDTO.md) |  | 
**UpdatedAt** | Pointer to **NullableTime** |  | [optional] 

## Methods

### NewDatasetDTO

`func NewDatasetDTO(name string, ownerTeam string, tags []string, sensitivity DatasetSensitivity, schemaFields []FieldDTO, ) *DatasetDTO`

NewDatasetDTO instantiates a new DatasetDTO object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDatasetDTOWithDefaults

`func NewDatasetDTOWithDefaults() *DatasetDTO`

NewDatasetDTOWithDefaults instantiates a new DatasetDTO object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *DatasetDTO) GetId() int64`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *DatasetDTO) GetIdOk() (*int64, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *DatasetDTO) SetId(v int64)`

SetId sets Id field to given value.

### HasId

`func (o *DatasetDTO) HasId() bool`

HasId returns a boolean if a field has been set.

### SetIdNil

`func (o *DatasetDTO) SetIdNil(b bool)`

 SetIdNil sets the value for Id to be an explicit nil

### UnsetId
`func (o *DatasetDTO) UnsetId()`

UnsetId ensures that no value is present for Id, not even an explicit nil
### GetName

`func (o *DatasetDTO) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *DatasetDTO) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *DatasetDTO) SetName(v string)`

SetName sets Name field to given value.


### GetOwnerTeam

`func (o *DatasetDTO) GetOwnerTeam() string`

GetOwnerTeam returns the OwnerTeam field if non-nil, zero value otherwise.

### GetOwnerTeamOk

`func (o *DatasetDTO) GetOwnerTeamOk() (*string, bool)`

GetOwnerTeamOk returns a tuple with the OwnerTeam field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOwnerTeam

`func (o *DatasetDTO) SetOwnerTeam(v string)`

SetOwnerTeam sets OwnerTeam field to given value.


### GetTags

`func (o *DatasetDTO) GetTags() []string`

GetTags returns the Tags field if non-nil, zero value otherwise.

### GetTagsOk

`func (o *DatasetDTO) GetTagsOk() (*[]string, bool)`

GetTagsOk returns a tuple with the Tags field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTags

`func (o *DatasetDTO) SetTags(v []string)`

SetTags sets Tags field to given value.


### GetSensitivity

`func (o *DatasetDTO) GetSensitivity() DatasetSensitivity`

GetSensitivity returns the Sensitivity field if non-nil, zero value otherwise.

### GetSensitivityOk

`func (o *DatasetDTO) GetSensitivityOk() (*DatasetSensitivity, bool)`

GetSensitivityOk returns a tuple with the Sensitivity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSensitivity

`func (o *DatasetDTO) SetSensitivity(v DatasetSensitivity)`

SetSensitivity sets Sensitivity field to given value.


### GetSchemaFields

`func (o *DatasetDTO) GetSchemaFields() []FieldDTO`

GetSchemaFields returns the SchemaFields field if non-nil, zero value otherwise.

### GetSchemaFieldsOk

`func (o *DatasetDTO) GetSchemaFieldsOk() (*[]FieldDTO, bool)`

GetSchemaFieldsOk returns a tuple with the SchemaFields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSchemaFields

`func (o *DatasetDTO) SetSchemaFields(v []FieldDTO)`

SetSchemaFields sets SchemaFields field to given value.


### GetUpdatedAt

`func (o *DatasetDTO) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *DatasetDTO) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *DatasetDTO) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *DatasetDTO) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.

### SetUpdatedAtNil

`func (o *DatasetDTO) SetUpdatedAtNil(b bool)`

 SetUpdatedAtNil sets the value for UpdatedAt to be an explicit nil

### UnsetUpdatedAt
`func (o *DatasetDTO) UnsetUpdatedAt()`

UnsetUpdatedAt ensures that no value is present for UpdatedAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


