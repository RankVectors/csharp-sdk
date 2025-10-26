# RankVectors.com.rankvectors.api.WebhooksApi

All URIs are relative to *https://api.rankvectors.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GetImplementationInstructions**](WebhooksApi.md#getimplementationinstructions) | **GET** /api/webhook/implement-link | Get implementation instructions |
| [**ReportImplementationStatus**](WebhooksApi.md#reportimplementationstatus) | **POST** /api/webhook/implement-link | Report implementation status |

<a id="getimplementationinstructions"></a>
# **GetImplementationInstructions**
> ImplementationInstructions GetImplementationInstructions (string suggestionId)

Get implementation instructions

Get step-by-step instructions for implementing a link


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **suggestionId** | **string** | ID of the suggestion to implement |  |

### Return type

[**ImplementationInstructions**](ImplementationInstructions.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Implementation instructions |  -  |
| **400** | Bad request - invalid parameters |  -  |
| **404** | Not found - resource doesn&#39;t exist |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="reportimplementationstatus"></a>
# **ReportImplementationStatus**
> ReportImplementationStatus200Response ReportImplementationStatus (ReportImplementationStatusRequest reportImplementationStatusRequest)

Report implementation status

Report the status of a link implementation


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **reportImplementationStatusRequest** | [**ReportImplementationStatusRequest**](ReportImplementationStatusRequest.md) |  |  |

### Return type

[**ReportImplementationStatus200Response**](ReportImplementationStatus200Response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Status reported successfully |  -  |
| **400** | Bad request - invalid parameters |  -  |
| **401** | Unauthorized - missing or invalid API key |  -  |
| **404** | Not found - resource doesn&#39;t exist |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

