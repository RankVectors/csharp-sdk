# RankVectors.com.rankvectors.api.CreditsApi

All URIs are relative to *https://api.rankvectors.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**AddCredits**](CreditsApi.md#addcredits) | **POST** /api/projects/{projectId}/credits | Add credits |
| [**GetCredits**](CreditsApi.md#getcredits) | **GET** /api/projects/{projectId}/credits | Get credit balance |

<a id="addcredits"></a>
# **AddCredits**
> AddCredits200Response AddCredits (string projectId, AddCreditsRequest addCreditsRequest)

Add credits

Add credits to a project (admin or payment webhook use)


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **projectId** | **string** | Unique identifier for the project |  |
| **addCreditsRequest** | [**AddCreditsRequest**](AddCreditsRequest.md) |  |  |

### Return type

[**AddCredits200Response**](AddCredits200Response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Credits added successfully |  -  |
| **400** | Bad request - invalid parameters |  -  |
| **401** | Unauthorized - missing or invalid API key |  -  |
| **403** | Forbidden - access denied to resource |  -  |
| **404** | Not found - resource doesn&#39;t exist |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getcredits"></a>
# **GetCredits**
> CreditBalance GetCredits (string projectId, bool includeHistory = null, DateTime startDate = null, DateTime endDate = null)

Get credit balance

Get credit balance and usage history for a project


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **projectId** | **string** | Unique identifier for the project |  |
| **includeHistory** | **bool** | Include usage history | [optional] [default to false] |
| **startDate** | **DateTime** | History start date (ISO 8601) | [optional]  |
| **endDate** | **DateTime** | History end date (ISO 8601) | [optional]  |

### Return type

[**CreditBalance**](CreditBalance.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Credit balance and usage information |  -  |
| **401** | Unauthorized - missing or invalid API key |  -  |
| **403** | Forbidden - access denied to resource |  -  |
| **404** | Not found - resource doesn&#39;t exist |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

