# RankVectors.com.rankvectors.model.Suggestion

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Unique suggestion identifier | 
**ProjectId** | **string** | Project identifier | 
**Status** | **string** | Suggestion status | 
**RelevanceScore** | **decimal** | AI-calculated relevance score (0-1) | 
**AnchorText** | **string** | Suggested anchor text | 
**SourcePage** | [**PageInfo**](PageInfo.md) |  | 
**TargetPage** | [**PageInfo**](PageInfo.md) |  | 
**CreatedAt** | **DateTime** | Suggestion creation timestamp | 
**Context** | **string** | Context where the link should be placed | [optional] 
**Reasoning** | **string** | AI reasoning for the suggestion | [optional] 
**UpdatedAt** | **DateTime** | Last update timestamp | [optional] 

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)

