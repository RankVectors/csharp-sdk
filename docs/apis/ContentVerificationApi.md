# RankVectors.com.rankvectors.api.ContentVerificationApi

All URIs are relative to *https://api.rankvectors.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**VerifyContent**](ContentVerificationApi.md#verifycontent) | **POST** /api/projects/{projectId}/verify-content | Verify page content |

<a id="verifycontent"></a>
# **VerifyContent**
> VerifyContent200Response VerifyContent (string projectId, VerifyContentRequest verifyContentRequest)

Verify page content

Check if page content has changed since last crawl


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **projectId** | **string** | Unique identifier for the project |  |
| **verifyContentRequest** | [**VerifyContentRequest**](VerifyContentRequest.md) |  |  |

### Return type

[**VerifyContent200Response**](VerifyContent200Response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Content verification result |  -  |
| **400** | Bad request - invalid parameters |  -  |
| **401** | Unauthorized - missing or invalid API key |  -  |
| **403** | Forbidden - access denied to resource |  -  |
| **404** | Not found - resource doesn&#39;t exist |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

