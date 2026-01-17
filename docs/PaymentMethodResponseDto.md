
# PaymentMethodResponseDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | Unique payment method identifier |  |
| **customerId** | **kotlin.String** | Customer ID this payment method belongs to |  |
| **type** | **kotlin.String** | Payment method type (e.g., card, mobile_money) |  |
| **provider** | **kotlin.String** | Payment provider name (e.g., iveri, mpesa) |  |
| **isDefault** | **kotlin.Boolean** | Whether this is the default payment method |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | When the payment method was created |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | When the payment method was last updated |  |
| **brand** | **kotlin.String** | Card brand (e.g., Visa, Mastercard) |  [optional] |
| **last4** | **kotlin.String** | Last 4 digits of card number |  [optional] |
| **expiryMonth** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Card expiry month (1-12) |  [optional] |
| **expiryYear** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Card expiry year |  [optional] |
| **phoneNumber** | **kotlin.String** | Phone number for mobile money |  [optional] |



