
# DebitReturnResponseDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **status** | [**inline**](#Status) | Payment status after 3DS authentication |  |
| **merchantReference** | **kotlin.String** | Merchant reference for the payment |  |
| **paymentIntentId** | **kotlin.String** | Payment intent ID |  [optional] |
| **transactionId** | **kotlin.String** | Transaction ID if payment succeeded |  [optional] |
| **authCode** | **kotlin.String** | Authorization code from payment gateway |  [optional] |
| **reason** | **kotlin.String** | Reason for failure if payment failed |  [optional] |
| **amount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Payment amount in smallest currency unit |  [optional] |
| **currency** | **kotlin.String** | Currency code |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | succeeded, failed, pending |



