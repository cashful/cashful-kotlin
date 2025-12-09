
# CreatePaymentIntentDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **customerId** | **kotlin.String** | The unique identifier of the customer |  |
| **paymentMethodId** | **kotlin.String** | The unique identifier of the payment method |  |
| **amount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | The amount to charge in the smallest currency unit |  |
| **currency** | **kotlin.String** | The three-letter ISO 4217 currency code |  |
| **metadata** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) | Optional custom metadata |  |
| **merchantId** | **kotlin.String** | The ID of the merchant whose balance is being requested. If omitted, defaults to the authenticated merchant. |  [optional] |
| **description** | **kotlin.String** | Optional description for the payment |  [optional] |



