# RankVectors.com.rankvectors.model.CreateProjectRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** | Project name | 
**Domain** | **string** | Website domain URL | 
**Prompt** | **string** | Natural language prompt for crawling | [optional] 
**SearchQuery** | **string** | Search query for targeted crawling | [optional] 
**SitemapMode** | **string** | How to handle sitemaps | [optional] [default to SitemapModeEnum.Include]
**IncludeSubdomains** | **bool** | Whether to include subdomains | [optional] [default to true]
**IgnoreQueryParams** | **bool** | Whether to ignore URL query parameters | [optional] [default to true]
**MaxDiscoveryDepth** | **int** | Maximum crawl depth | [optional] 
**ExcludePaths** | **List&lt;string&gt;** | Paths to exclude from crawling | [optional] 
**IncludePaths** | **List&lt;string&gt;** | Specific paths to include | [optional] 
**CrawlEntireDomain** | **bool** | Whether to crawl the entire domain | [optional] [default to false]
**AllowExternalLinks** | **bool** | Whether to allow external links | [optional] [default to false]
**MaxPages** | **int** | Maximum number of pages to crawl | [optional] [default to 100]
**CrawlDelay** | **int** | Delay between crawl requests (ms) | [optional] 
**CrawlMaxConcurrency** | **int** | Maximum concurrent crawl requests | [optional] 
**OnlyMainContent** | **bool** | Whether to extract only main content | [optional] [default to true]
**CustomHeaders** | **Dictionary&lt;string, string&gt;** | Custom headers for crawling | [optional] 
**WaitFor** | **int** | Wait time for page load (ms) | [optional] [default to 0]
**BlockAds** | **bool** | Whether to block ads | [optional] [default to true]
**ProxyMode** | **string** | Proxy mode for crawling | [optional] [default to ProxyModeEnum.Auto]
**UseReranking** | **bool** | Whether to use AI reranking | [optional] [default to true]
**EnableChangeTracking** | **bool** | Whether to enable change tracking | [optional] [default to false]

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)

