
# PaymentIntentResponseDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | Unique payment intent ID |  |
| **merchantId** | **kotlin.String** | Merchant ID |  |
| **customerId** | **kotlin.String** | Customer ID (if associated) |  |
| **paymentMethodId** | **kotlin.String** | Payment method ID (if attached) |  |
| **amount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Amount in smallest currency unit |  |
| **currency** | **kotlin.String** | Three-letter currency code |  |
| **status** | [**inline**](#Status) | Current status of the payment intent |  |
| **mode** | [**inline**](#Mode) | Mode of the payment intent |  |
| **idempotencyKey** | **kotlin.String** | Unique idempotency key for this payment intent |  |
| **expiresAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | When the payment intent expires |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Creation timestamp |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Last update timestamp |  |
| **description** | **kotlin.String** | Description |  [optional] |
| **metadata** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) | Custom metadata |  [optional] |
| **deletedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Deletion timestamp (for soft deletes) |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | initiation, requires_payment_method, requires_confirmation, requires_action, processing, requires_capture, succeeded, failed, canceled |


<a id="Mode"></a>
## Enum: mode
| Name | Value |
| ---- | ----- |
| mode | payment, setup, subscription |



