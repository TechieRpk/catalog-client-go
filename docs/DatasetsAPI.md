# \DatasetsAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateDataset**](DatasetsAPI.md#CreateDataset) | **Post** /datasets | 
[**DeleteDataset**](DatasetsAPI.md#DeleteDataset) | **Delete** /datasets/{id} | 
[**GetDataset**](DatasetsAPI.md#GetDataset) | **Get** /datasets/{id} | 
[**ListDatasets**](DatasetsAPI.md#ListDatasets) | **Get** /datasets | 
[**UpdateDataset**](DatasetsAPI.md#UpdateDataset) | **Put** /datasets/{id} | 



## CreateDataset

> DatasetDTO CreateDataset(ctx).DatasetDTO(datasetDTO).Execute()



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/javazone-2026/catalog-client-go"
)

func main() {
	datasetDTO := *openapiclient.NewDatasetDTO("Name_example", "OwningTeam_example", "SourceSystem_example", []string{"Tags_example"}, openapiclient.DatasetSensitivity("PUBLIC"), int32(123), int32(123), []openapiclient.FieldDTO{*openapiclient.NewFieldDTO("Name_example", "Type_example")}) // DatasetDTO | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DatasetsAPI.CreateDataset(context.Background()).DatasetDTO(datasetDTO).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DatasetsAPI.CreateDataset``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateDataset`: DatasetDTO
	fmt.Fprintf(os.Stdout, "Response from `DatasetsAPI.CreateDataset`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateDatasetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **datasetDTO** | [**DatasetDTO**](DatasetDTO.md) |  | 

### Return type

[**DatasetDTO**](DatasetDTO.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteDataset

> DeleteDataset(ctx, id).Execute()



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/javazone-2026/catalog-client-go"
)

func main() {
	id := int64(789) // int64 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.DatasetsAPI.DeleteDataset(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DatasetsAPI.DeleteDataset``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int64** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteDatasetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetDataset

> DatasetDTO GetDataset(ctx, id).Execute()



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/javazone-2026/catalog-client-go"
)

func main() {
	id := int64(789) // int64 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DatasetsAPI.GetDataset(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DatasetsAPI.GetDataset``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDataset`: DatasetDTO
	fmt.Fprintf(os.Stdout, "Response from `DatasetsAPI.GetDataset`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int64** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetDatasetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**DatasetDTO**](DatasetDTO.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListDatasets

> []DatasetDTO ListDatasets(ctx).Execute()



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/javazone-2026/catalog-client-go"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DatasetsAPI.ListDatasets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DatasetsAPI.ListDatasets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDatasets`: []DatasetDTO
	fmt.Fprintf(os.Stdout, "Response from `DatasetsAPI.ListDatasets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListDatasetsRequest struct via the builder pattern


### Return type

[**[]DatasetDTO**](DatasetDTO.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateDataset

> DatasetDTO UpdateDataset(ctx, id).DatasetDTO(datasetDTO).Execute()



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/javazone-2026/catalog-client-go"
)

func main() {
	id := int64(789) // int64 | 
	datasetDTO := *openapiclient.NewDatasetDTO("Name_example", "OwningTeam_example", "SourceSystem_example", []string{"Tags_example"}, openapiclient.DatasetSensitivity("PUBLIC"), int32(123), int32(123), []openapiclient.FieldDTO{*openapiclient.NewFieldDTO("Name_example", "Type_example")}) // DatasetDTO | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DatasetsAPI.UpdateDataset(context.Background(), id).DatasetDTO(datasetDTO).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DatasetsAPI.UpdateDataset``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateDataset`: DatasetDTO
	fmt.Fprintf(os.Stdout, "Response from `DatasetsAPI.UpdateDataset`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int64** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateDatasetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **datasetDTO** | [**DatasetDTO**](DatasetDTO.md) |  | 

### Return type

[**DatasetDTO**](DatasetDTO.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

