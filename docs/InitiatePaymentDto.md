
# InitiatePaymentDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **amount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Payment amount in the smallest currency unit (e.g., cents) |  |
| **currency** | **kotlin.String** | Three-letter ISO 4217 currency code |  |
| **merchantId** | **kotlin.String** | The unique identifier of the merchant |  |
| **evervaultEncryptedCard** | [**EvervaultEncryptedCardDto**](EvervaultEncryptedCardDto.md) | Evervault encrypted card details |  |
| **paymentIntentId** | **kotlin.String** | Payment intent ID (generated if not provided) |  [optional] |
| **maskedPan** | **kotlin.String** | Masked PAN for display purposes |  [optional] |
| **tokenizeCard** | **kotlin.Boolean** | Whether to tokenize the card for future use |  [optional] |
| **firstName** | **kotlin.String** | Cardholder first name |  [optional] |
| **lastName** | **kotlin.String** | Cardholder last name |  [optional] |
| **phoneNumber** | **kotlin.String** | Cardholder phone number |  [optional] |
| **paymentDescription** | **kotlin.String** | Payment description |  [optional] |
| **merchantName** | **kotlin.String** | Merchant name for display |  [optional] |
| **metadata** | [**kotlin.Any**](.md) | Additional metadata |  [optional] |



