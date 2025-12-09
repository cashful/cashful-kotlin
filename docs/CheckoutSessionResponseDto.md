
# CheckoutSessionResponseDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | Unique identifier |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  |
| **merchantId** | **kotlin.String** |  |  |
| **sessionUrl** | **kotlin.String** |  |  |
| **successUrl** | **kotlin.String** |  |  |
| **cancelUrl** | **kotlin.String** |  |  |
| **currency** | **kotlin.String** |  |  |
| **status** | **kotlin.String** |  |  |
| **metadata** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) |  |  |
| **deletedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **customerId** | **kotlin.String** |  |  [optional] |
| **lineItems** | [**kotlin.collections.List&lt;LineItemDto&gt;**](LineItemDto.md) |  |  [optional] |
| **totalAmount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **mode** | **kotlin.String** |  |  [optional] |
| **expiresAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |



