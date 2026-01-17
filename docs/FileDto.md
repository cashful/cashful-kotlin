
# FileDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | Unique identifier |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  |
| **key** | **kotlin.String** |  |  |
| **bucket** | **kotlin.String** |  |  |
| **filename** | **kotlin.String** |  |  |
| **mimeType** | **kotlin.String** |  |  |
| **propertySize** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  |
| **tags** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  |
| **status** | [**inline**](#Status) |  |  |
| **isPublic** | **kotlin.Boolean** |  |  |
| **deletedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **checksum** | **kotlin.String** |  |  [optional] |
| **relatedEntityId** | **kotlin.String** |  |  [optional] |
| **relatedEntityType** | **kotlin.String** |  |  [optional] |
| **uploadedById** | **kotlin.String** |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | pending, uploaded, failed, deleted |



