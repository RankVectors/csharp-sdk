# RankVectors.com.rankvectors.api.CrawlingApi

All URIs are relative to *https://api.rankvectors.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GetCrawlHistory**](CrawlingApi.md#getcrawlhistory) | **GET** /api/projects/{projectId}/crawl | Get crawl history |
| [**StartCrawl**](CrawlingApi.md#startcrawl) | **POST** /api/projects/{projectId}/crawl | Start website crawl |

<a id="getcrawlhistory"></a>
# **GetCrawlHistory**
> List&lt;Crawl&gt; GetCrawlHistory (string projectId)

Get crawl history

Get the crawl history for a project


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **projectId** | **string** | Unique identifier for the project |  |

### Return type

[**List&lt;Crawl&gt;**](Crawl.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Crawl history |  -  |
| **401** | Unauthorized - missing or invalid API key |  -  |
| **403** | Forbidden - access denied to resource |  -  |
| **404** | Not found - resource doesn&#39;t exist |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="startcrawl"></a>
# **StartCrawl**
> Crawl StartCrawl (string projectId, StartCrawlRequest startCrawlRequest = null)

Start website crawl

Start crawling a website to analyze content for link opportunities


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **projectId** | **string** | Unique identifier for the project |  |
| **startCrawlRequest** | [**StartCrawlRequest**](StartCrawlRequest.md) |  | [optional]  |

### Return type

[**Crawl**](Crawl.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Crawl started successfully |  -  |
| **401** | Unauthorized - missing or invalid API key |  -  |
| **403** | Forbidden - access denied to resource |  -  |
| **404** | Not found - resource doesn&#39;t exist |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

