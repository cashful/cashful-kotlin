
# CreatePaymentLinkDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **currency** | **kotlin.String** | The three-letter ISO 4217 currency code |  |
| **mode** | **kotlin.String** | The payment mode (e.g., &#39;payment&#39; or &#39;subscription&#39;) |  |
| **successUrl** | **kotlin.String** | The URL to redirect to on successful payment |  |
| **cancelUrl** | **kotlin.String** | The URL to redirect to if customer cancels |  |
| **metadata** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) | Optional custom metadata |  |
| **merchantId** | **kotlin.String** | The ID of the merchant whose balance is being requested. If omitted, defaults to the authenticated merchant. |  [optional] |
| **productId** | **kotlin.String** | The unique identifier of the product |  [optional] |
| **customerId** | **kotlin.String** | The unique identifier of the customer |  [optional] |
| **amount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | The amount in the smallest currency unit |  [optional] |



