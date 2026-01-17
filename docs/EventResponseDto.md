
# EventResponseDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | Unique identifier for the event |  |
| **merchantId** | **kotlin.String** | ID of the merchant this event belongs to |  |
| **webhookEndpointId** | **kotlin.String** | ID of the webhook endpoint this event was sent to |  |
| **type** | **kotlin.String** | Event type name |  |
| **&#x60;data&#x60;** | [**kotlin.Any**](.md) | Event data payload |  |
| **status** | [**inline**](#Status) | Current delivery status of the event |  |
| **attempts** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Number of delivery attempts |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the event was created |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the event was last updated |  |
| **relatedEntityId** | **kotlin.String** | ID of the related entity |  [optional] |
| **relatedEntityType** | **kotlin.String** | Type of the related entity |  [optional] |
| **lastAttemptAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp of the last delivery attempt |  [optional] |
| **nextRetryAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp for the next retry attempt |  [optional] |
| **deliveredAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp when the event was successfully delivered |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | pending, delivered, failed |



