# RankVectors.com.rankvectors.model.Implementation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Unique implementation identifier | 
**Status** | **string** | Implementation status | 
**Platform** | **string** | Platform used | 
**CreditsUsed** | **decimal** | Credits consumed | 
**CreatedAt** | **DateTime** | Implementation start timestamp | 
**Suggestion** | [**Suggestion**](Suggestion.md) |  | 
**ImplementationMethod** | **string** | Implementation method | [optional] 
**CompletedAt** | **DateTime** | Implementation completion timestamp | [optional] 
**Metadata** | **Dictionary&lt;string, Object&gt;** | Platform-specific metadata | [optional] 
**Rollbacks** | [**List&lt;Rollback&gt;**](Rollback.md) | Rollback history | [optional] 

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)

