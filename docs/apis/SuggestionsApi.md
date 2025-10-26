# RankVectors.com.rankvectors.api.SuggestionsApi

All URIs are relative to *https://api.rankvectors.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GenerateSuggestions**](SuggestionsApi.md#generatesuggestions) | **POST** /api/projects/{projectId}/suggestions | Generate link suggestions |
| [**GetSuggestions**](SuggestionsApi.md#getsuggestions) | **GET** /api/projects/{projectId}/suggestions | Get link suggestions |
| [**UpdateSuggestion**](SuggestionsApi.md#updatesuggestion) | **PATCH** /api/projects/{projectId}/suggestions/{suggestionId} | Update suggestion status |

<a id="generatesuggestions"></a>
# **GenerateSuggestions**
> GenerateSuggestions200Response GenerateSuggestions (string projectId, GenerateSuggestionsRequest generateSuggestionsRequest = null)

Generate link suggestions

Generate new AI-powered link suggestions for a project


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **projectId** | **string** | Unique identifier for the project |  |
| **generateSuggestionsRequest** | [**GenerateSuggestionsRequest**](GenerateSuggestionsRequest.md) |  | [optional]  |

### Return type

[**GenerateSuggestions200Response**](GenerateSuggestions200Response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Suggestions generated successfully |  -  |
| **401** | Unauthorized - missing or invalid API key |  -  |
| **403** | Forbidden - access denied to resource |  -  |
| **404** | Not found - resource doesn&#39;t exist |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getsuggestions"></a>
# **GetSuggestions**
> List&lt;Suggestion&gt; GetSuggestions (string projectId, string status = null)

Get link suggestions

Get AI-generated link suggestions for a project


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **projectId** | **string** | Unique identifier for the project |  |
| **status** | **string** | Filter suggestions by status | [optional]  |

### Return type

[**List&lt;Suggestion&gt;**](Suggestion.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of link suggestions |  -  |
| **401** | Unauthorized - missing or invalid API key |  -  |
| **403** | Forbidden - access denied to resource |  -  |
| **404** | Not found - resource doesn&#39;t exist |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="updatesuggestion"></a>
# **UpdateSuggestion**
> Suggestion UpdateSuggestion (string projectId, string suggestionId, UpdateSuggestionRequest updateSuggestionRequest)

Update suggestion status

Update the status of a link suggestion


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **projectId** | **string** | Unique identifier for the project |  |
| **suggestionId** | **string** | Unique identifier for the suggestion |  |
| **updateSuggestionRequest** | [**UpdateSuggestionRequest**](UpdateSuggestionRequest.md) |  |  |

### Return type

[**Suggestion**](Suggestion.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Suggestion updated successfully |  -  |
| **400** | Bad request - invalid parameters |  -  |
| **401** | Unauthorized - missing or invalid API key |  -  |
| **403** | Forbidden - access denied to resource |  -  |
| **404** | Not found - resource doesn&#39;t exist |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

