# RankVectors.com.rankvectors.api.ImplementationsApi

All URIs are relative to *https://api.rankvectors.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GetImplementation**](ImplementationsApi.md#getimplementation) | **GET** /api/projects/{projectId}/implementations/{implementationId} | Get implementation details |
| [**ImplementLinks**](ImplementationsApi.md#implementlinks) | **POST** /api/projects/{projectId}/implementations | Implement link suggestions |
| [**ListImplementations**](ImplementationsApi.md#listimplementations) | **GET** /api/projects/{projectId}/implementations | List implementations |
| [**RollbackImplementation**](ImplementationsApi.md#rollbackimplementation) | **POST** /api/projects/{projectId}/implementations/{implementationId}/rollback | Rollback implementation |

<a id="getimplementation"></a>
# **GetImplementation**
> GetImplementation200Response GetImplementation (string projectId, string implementationId)

Get implementation details

Get detailed information about a specific implementation


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **projectId** | **string** | Unique identifier for the project |  |
| **implementationId** | **string** | Unique identifier for the implementation |  |

### Return type

[**GetImplementation200Response**](GetImplementation200Response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Implementation details |  -  |
| **401** | Unauthorized - missing or invalid API key |  -  |
| **403** | Forbidden - access denied to resource |  -  |
| **404** | Not found - resource doesn&#39;t exist |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="implementlinks"></a>
# **ImplementLinks**
> ImplementationResponse ImplementLinks (string projectId, ImplementationRequest implementationRequest)

Implement link suggestions

Implement one or more link suggestions


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **projectId** | **string** | Unique identifier for the project |  |
| **implementationRequest** | [**ImplementationRequest**](ImplementationRequest.md) |  |  |

### Return type

[**ImplementationResponse**](ImplementationResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Implementation results |  -  |
| **400** | Bad request - invalid parameters |  -  |
| **401** | Unauthorized - missing or invalid API key |  -  |
| **402** | Payment required - insufficient credits |  -  |
| **403** | Forbidden - access denied to resource |  -  |
| **404** | Not found - resource doesn&#39;t exist |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="listimplementations"></a>
# **ListImplementations**
> ListImplementations200Response ListImplementations (string projectId, string status = null, string platform = null, int limit = null, int offset = null)

List implementations

Get implementation history for a project


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **projectId** | **string** | Unique identifier for the project |  |
| **status** | **string** | Filter by implementation status | [optional]  |
| **platform** | **string** | Filter by platform | [optional]  |
| **limit** | **int** | Results per page | [optional] [default to 50] |
| **offset** | **int** | Pagination offset | [optional] [default to 0] |

### Return type

[**ListImplementations200Response**](ListImplementations200Response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Implementation history |  -  |
| **401** | Unauthorized - missing or invalid API key |  -  |
| **403** | Forbidden - access denied to resource |  -  |
| **404** | Not found - resource doesn&#39;t exist |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="rollbackimplementation"></a>
# **RollbackImplementation**
> RollbackImplementation200Response RollbackImplementation (string projectId, string implementationId, RollbackImplementationRequest rollbackImplementationRequest)

Rollback implementation

Undo a link implementation and restore original content


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **projectId** | **string** | Unique identifier for the project |  |
| **implementationId** | **string** | Unique identifier for the implementation |  |
| **rollbackImplementationRequest** | [**RollbackImplementationRequest**](RollbackImplementationRequest.md) |  |  |

### Return type

[**RollbackImplementation200Response**](RollbackImplementation200Response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Rollback successful |  -  |
| **400** | Bad request - invalid parameters |  -  |
| **401** | Unauthorized - missing or invalid API key |  -  |
| **403** | Forbidden - access denied to resource |  -  |
| **404** | Not found - resource doesn&#39;t exist |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

