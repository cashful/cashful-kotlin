
# CreateCheckoutSessionDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **currency** | **kotlin.String** | The three-letter ISO 4217 currency code |  |
| **metadata** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) | Optional custom metadata |  |
| **merchantId** | **kotlin.String** | The ID of the merchant whose balance is being requested. If omitted, defaults to the authenticated merchant. |  [optional] |
| **customerId** | **kotlin.String** | The unique identifier of the customer |  [optional] |
| **productId** | **kotlin.String** | The unique identifier of the product |  [optional] |
| **successUrl** | **kotlin.String** | The URL to redirect to on successful payment |  [optional] |
| **failureUrl** | **kotlin.String** | The URL to redirect to on failure |  [optional] |
| **cancelUrl** | **kotlin.String** | The URL to redirect to on cancel |  [optional] |
| **lineItems** | [**kotlin.collections.List&lt;LineItemDto&gt;**](LineItemDto.md) | Array of line items for the checkout |  [optional] |
| **totalAmount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | The total amount in the smallest currency unit |  [optional] |
| **mode** | **kotlin.String** | The checkout mode (e.g., &#39;payment&#39;) |  [optional] |
| **hostedCheckoutConfig** | [**HostedCheckoutConfigDto**](HostedCheckoutConfigDto.md) | Configuration for the hosted checkout page |  [optional] |



