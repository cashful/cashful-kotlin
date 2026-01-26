
# PaymentLinkResponseDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  |
| **merchantId** | **kotlin.String** |  |  |
| **url** | **kotlin.String** |  |  |
| **totalAmount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  |
| **currency** | **kotlin.String** |  |  |
| **mode** | [**inline**](#Mode) |  |  |
| **active** | **kotlin.Boolean** |  |  |
| **successUrl** | **kotlin.String** |  |  |
| **cancelUrl** | **kotlin.String** |  |  |
| **metadata** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) |  |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  |
| **name** | **kotlin.String** |  |  [optional] |
| **description** | **kotlin.String** |  |  [optional] |
| **lineItems** | [**kotlin.collections.List&lt;LineItemDto&gt;**](LineItemDto.md) |  |  [optional] |
| **customerId** | **kotlin.String** |  |  [optional] |
| **hostedCheckoutConfig** | [**HostedCheckoutConfigDto**](HostedCheckoutConfigDto.md) | Configuration for the hosted checkout page |  [optional] |
| **deletedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Mode"></a>
## Enum: mode
| Name | Value |
| ---- | ----- |
| mode | payment, setup, subscription |



