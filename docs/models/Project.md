# RankVectors.com.rankvectors.model.Project

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Unique project identifier | 
**Name** | **string** | Project name | 
**Domain** | **string** | Website domain URL | 
**UserId** | **string** | User who owns the project | 
**CreatedAt** | **DateTime** | Project creation timestamp | 
**UpdatedAt** | **DateTime** | Last update timestamp | 
**Prompt** | **string** | Natural language prompt for crawling | [optional] 
**SearchQuery** | **string** | Search query for targeted crawling | [optional] 
**SitemapMode** | **string** | How to handle sitemaps | [optional] 
**IncludeSubdomains** | **bool** | Whether to include subdomains | [optional] 
**IgnoreQueryParams** | **bool** | Whether to ignore URL query parameters | [optional] 
**MaxDiscoveryDepth** | **int** | Maximum crawl depth | [optional] 
**ExcludePaths** | **List&lt;string&gt;** | Paths to exclude from crawling | [optional] 
**IncludePaths** | **List&lt;string&gt;** | Specific paths to include | [optional] 
**CrawlEntireDomain** | **bool** | Whether to crawl the entire domain | [optional] 
**AllowExternalLinks** | **bool** | Whether to allow external links | [optional] 
**MaxPages** | **int** | Maximum number of pages to crawl | [optional] 
**CrawlDelay** | **int** | Delay between crawl requests (ms) | [optional] 
**CrawlMaxConcurrency** | **int** | Maximum concurrent crawl requests | [optional] 
**OnlyMainContent** | **bool** | Whether to extract only main content | [optional] 
**CustomHeaders** | **Dictionary&lt;string, string&gt;** | Custom headers for crawling | [optional] 
**WaitFor** | **int** | Wait time for page load (ms) | [optional] 
**BlockAds** | **bool** | Whether to block ads | [optional] 
**ProxyMode** | **string** | Proxy mode for crawling | [optional] 
**UseReranking** | **bool** | Whether to use AI reranking | [optional] 
**EnableChangeTracking** | **bool** | Whether to enable change tracking | [optional] 
**Count** | [**ProjectCount**](ProjectCount.md) |  | [optional] 

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)

