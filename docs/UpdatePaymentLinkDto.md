
# UpdatePaymentLinkDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **metadata** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) | Optional custom metadata |  |
| **name** | **kotlin.String** | The name of the payment link |  [optional] |
| **description** | **kotlin.String** | A description of the payment link |  [optional] |
| **active** | **kotlin.Boolean** | Whether the payment link is active |  [optional] |
| **totalAmount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **successUrl** | **kotlin.String** | The URL to redirect to on successful payment |  [optional] |
| **cancelUrl** | **kotlin.String** | The URL to redirect to if customer cancels |  [optional] |
| **hostedCheckoutConfig** | [**HostedCheckoutConfigDto**](HostedCheckoutConfigDto.md) | Configuration for the hosted checkout page |  [optional] |



