
# CreateProductDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** | The name of the product |  |
| **currency** | **kotlin.String** | The three-letter ISO 4217 currency code |  |
| **metadata** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) | Optional custom metadata |  |
| **merchantId** | **kotlin.String** | The ID of the merchant whose balance is being requested. If omitted, defaults to the authenticated merchant. |  [optional] |
| **description** | **kotlin.String** | A description of the product |  [optional] |
| **amount** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | The price of the product in the smallest currency unit |  [optional] |
| **active** | **kotlin.Boolean** | Whether the product is active |  [optional] |
| **imageId** | **kotlin.String** | The ID of the product image file |  [optional] |



