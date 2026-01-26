
# CreatePaymentLinkDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **totalAmount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | The total amount in the smallest currency unit |  |
| **currency** | **kotlin.String** | The three-letter ISO 4217 currency code |  |
| **mode** | [**inline**](#Mode) | The payment mode (e.g., &#39;payment&#39; or &#39;subscription&#39;) |  |
| **successUrl** | **kotlin.String** | The URL to redirect to on successful payment |  |
| **cancelUrl** | **kotlin.String** | The URL to redirect to if customer cancels |  |
| **metadata** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) | Optional custom metadata |  |
| **name** | **kotlin.String** | The name of the payment link |  [optional] |
| **description** | **kotlin.String** | A description of the payment link |  [optional] |
| **merchantId** | **kotlin.String** | The ID of the merchant whose balance is being requested. If omitted, defaults to the authenticated merchant. |  [optional] |
| **lineItems** | [**kotlin.collections.List&lt;LineItemDto&gt;**](LineItemDto.md) | Array of line items for the checkout |  [optional] |
| **customerId** | **kotlin.String** | The unique identifier of the customer |  [optional] |
| **hostedCheckoutConfig** | [**HostedCheckoutConfigDto**](HostedCheckoutConfigDto.md) | Configuration for the hosted checkout page |  [optional] |


<a id="Mode"></a>
## Enum: mode
| Name | Value |
| ---- | ----- |
| mode | payment, setup, subscription |



