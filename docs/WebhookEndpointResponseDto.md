
# WebhookEndpointResponseDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | Unique identifier for the webhook endpoint |  |
| **merchantId** | **kotlin.String** | The merchant ID this webhook belongs to |  |
| **url** | **kotlin.String** | The URL where webhook events are sent |  |
| **events** | **kotlin.collections.List&lt;kotlin.String&gt;** | Array of event types subscribed to |  |
| **active** | **kotlin.Boolean** | Whether the webhook endpoint is active |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | When the webhook endpoint was created |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | When the webhook endpoint was last updated |  |
| **metadata** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) | Custom metadata attached to the webhook endpoint |  [optional] |
| **deletedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | When the webhook endpoint was deleted (soft delete) |  [optional] |



