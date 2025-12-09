
# CreatePurchaseDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **customerId** | **kotlin.String** | The unique identifier of the customer |  |
| **productId** | **kotlin.String** | The unique identifier of the product |  |
| **amount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | The amount in the smallest currency unit |  |
| **currency** | **kotlin.String** | The three-letter ISO 4217 currency code |  |
| **merchantId** | **kotlin.String** | The ID of the merchant whose balance is being requested. If omitted, defaults to the authenticated merchant. |  [optional] |
| **quantity** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | The quantity of items in the purchase |  [optional] |



