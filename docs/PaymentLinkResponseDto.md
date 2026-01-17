
# PaymentLinkResponseDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  |
| **merchantId** | **kotlin.String** |  |  |
| **url** | **kotlin.String** |  |  |
| **currency** | **kotlin.String** |  |  |
| **mode** | [**inline**](#Mode) |  |  |
| **active** | **kotlin.Boolean** |  |  |
| **successUrl** | **kotlin.String** |  |  |
| **cancelUrl** | **kotlin.String** |  |  |
| **metadata** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) |  |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  |
| **productId** | **kotlin.String** |  |  [optional] |
| **customerId** | **kotlin.String** |  |  [optional] |
| **amount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **deletedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Mode"></a>
## Enum: mode
| Name | Value |
| ---- | ----- |
| mode | payment, setup, subscription |



