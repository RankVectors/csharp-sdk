# RankVectors.com.rankvectors.api.ProjectsApi

All URIs are relative to *https://api.rankvectors.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CreateProject**](ProjectsApi.md#createproject) | **POST** /api/projects | Create a new project |
| [**DeleteProject**](ProjectsApi.md#deleteproject) | **DELETE** /api/projects/{projectId} | Delete a project |
| [**GetProject**](ProjectsApi.md#getproject) | **GET** /api/projects/{projectId} | Get project details |
| [**ListProjects**](ProjectsApi.md#listprojects) | **GET** /api/projects | List all projects |

<a id="createproject"></a>
# **CreateProject**
> Project CreateProject (CreateProjectRequest createProjectRequest)

Create a new project

Create a new project for internal linking optimization


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **createProjectRequest** | [**CreateProjectRequest**](CreateProjectRequest.md) |  |  |

### Return type

[**Project**](Project.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Project created successfully |  -  |
| **400** | Bad request - invalid parameters |  -  |
| **401** | Unauthorized - missing or invalid API key |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="deleteproject"></a>
# **DeleteProject**
> DeleteProject200Response DeleteProject (string projectId)

Delete a project

Delete a project and all associated data


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **projectId** | **string** | Unique identifier for the project |  |

### Return type

[**DeleteProject200Response**](DeleteProject200Response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Project deleted successfully |  -  |
| **401** | Unauthorized - missing or invalid API key |  -  |
| **403** | Forbidden - access denied to resource |  -  |
| **404** | Not found - resource doesn&#39;t exist |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getproject"></a>
# **GetProject**
> Project GetProject (string projectId)

Get project details

Get detailed information about a specific project


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **projectId** | **string** | Unique identifier for the project |  |

### Return type

[**Project**](Project.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Project details |  -  |
| **401** | Unauthorized - missing or invalid API key |  -  |
| **403** | Forbidden - access denied to resource |  -  |
| **404** | Not found - resource doesn&#39;t exist |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="listprojects"></a>
# **ListProjects**
> List&lt;Project&gt; ListProjects ()

List all projects

Get a list of all projects for the authenticated user


### Parameters
This endpoint does not need any parameter.
### Return type

[**List&lt;Project&gt;**](Project.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of projects |  -  |
| **401** | Unauthorized - missing or invalid API key |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

