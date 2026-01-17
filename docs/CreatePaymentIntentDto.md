
# CreatePaymentIntentDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **amount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | The amount to charge in the smallest currency unit (cents) |  |
| **currency** | **kotlin.String** | The three-letter ISO 4217 currency code |  |
| **merchantId** | **kotlin.String** | The ID of the merchant whose balance is being requested. If omitted, defaults to the authenticated merchant. |  [optional] |
| **customerId** | **kotlin.String** | The unique identifier of the customer. Optional for payment intents that don&#39;t require a customer. |  [optional] |
| **paymentMethodId** | **kotlin.String** | The unique identifier of the payment method. Optional if payment method will be collected later. |  [optional] |
| **mode** | [**inline**](#Mode) | The mode of the payment intent |  [optional] |
| **description** | **kotlin.String** | Optional description for the payment |  [optional] |
| **metadata** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) | Optional custom metadata |  [optional] |
| **idempotencyKey** | **kotlin.String** | A unique key to prevent duplicate charges. If not provided, one will be generated. |  [optional] |
| **expiresAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | When the payment intent expires. Defaults to 24 hours from creation. |  [optional] |


<a id="Mode"></a>
## Enum: mode
| Name | Value |
| ---- | ----- |
| mode | payment, setup, subscription |



