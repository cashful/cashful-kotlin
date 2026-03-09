
# CheckoutSessionConfirmResponseDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **sessionId** | **kotlin.String** |  |  |
| **paymentIntentId** | **kotlin.String** |  |  |
| **iveriParams** | [**kotlin.Any**](.md) |  |  [optional] |
| **iVeri3dsEndpoint** | **kotlin.String** |  |  [optional] |
| **sandboxMode** | **kotlin.Boolean** |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **transactionId** | **kotlin.String** |  |  [optional] |
| **authCode** | **kotlin.String** |  |  [optional] |
| **amount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **currency** | **kotlin.String** |  |  [optional] |
| **reason** | **kotlin.String** |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | succeeded, failed |



