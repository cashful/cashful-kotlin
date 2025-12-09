
# CreateTransferDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **fromCustomerId** | **kotlin.String** | The unique identifier of the customer sending the transfer |  |
| **toCustomerId** | **kotlin.String** | The unique identifier of the customer receiving the transfer |  |
| **amount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | The amount to transfer in the smallest currency unit |  |
| **currency** | **kotlin.String** | The three-letter ISO 4217 currency code |  |
| **merchantId** | **kotlin.String** | The ID of the merchant whose balance is being requested. If omitted, defaults to the authenticated merchant. |  [optional] |
| **description** | **kotlin.String** | Optional description for the transfer |  [optional] |



