
# InitiatePaymentResponseDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **iveriParams** | [**IveriParamsDto**](IveriParamsDto.md) | Parameters to POST to iVeri 3DS endpoint (only in live mode) |  [optional] |
| **iVeri3dsEndpoint** | **kotlin.String** | iVeri 3DS endpoint URL to POST the parameters to (only in live mode) |  [optional] |
| **sandboxMode** | **kotlin.Boolean** | Whether sandbox mode is active |  [optional] |
| **status** | [**inline**](#Status) | Payment status (only in sandbox mode) |  [optional] |
| **paymentIntentId** | **kotlin.String** | Payment intent ID |  [optional] |
| **transactionId** | **kotlin.String** | Transaction ID (only in sandbox mode on success) |  [optional] |
| **authCode** | **kotlin.String** | Authorization code (only in sandbox mode on success) |  [optional] |
| **amount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Payment amount in smallest currency unit |  [optional] |
| **currency** | **kotlin.String** | Currency code |  [optional] |
| **reason** | **kotlin.String** | Reason for failure (only in sandbox mode on failure) |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | succeeded, failed |



