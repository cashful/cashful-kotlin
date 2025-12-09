# ProductsApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createProduct**](ProductsApi.md#createProduct) | **POST** /api/canary/products | Create Product |
| [**listProducts**](ProductsApi.md#listProducts) | **GET** /api/canary/products | List Products |
| [**updateProduct**](ProductsApi.md#updateProduct) | **PATCH** /api/canary/products/{id} | Update Product |


<a id="createProduct"></a>
# **createProduct**
> ProductResponseDto createProduct(createProductDto)

Create Product

Defines a product in the merchant&#39;s catalog (e.g., \&quot;Airtime,\&quot; \&quot;Data\&quot;).

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = ProductsApi()
val createProductDto : CreateProductDto =  // CreateProductDto | Product details
try {
    val result : ProductResponseDto = apiInstance.createProduct(createProductDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductsApi#createProduct")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductsApi#createProduct")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createProductDto** | [**CreateProductDto**](CreateProductDto.md)| Product details | |

### Return type

[**ProductResponseDto**](ProductResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="listProducts"></a>
# **listProducts**
> ListProductsResponseDto listProducts(merchantId, active, limit, offset)

List Products

Retrieves all products in the merchant&#39;s catalog.

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = ProductsApi()
val merchantId : kotlin.String = merchantId_example // kotlin.String | The ID of the merchant. This parameter is required.
val active : kotlin.Boolean = true // kotlin.Boolean | Filter by active status
val limit : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Maximum number of records to return
val offset : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Number of records to skip
try {
    val result : ListProductsResponseDto = apiInstance.listProducts(merchantId, active, limit, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductsApi#listProducts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductsApi#listProducts")
    e.printStackTrace()
}
```

### Parameters
| **merchantId** | **kotlin.String**| The ID of the merchant. This parameter is required. | |
| **active** | **kotlin.Boolean**| Filter by active status | [optional] |
| **limit** | **java.math.BigDecimal**| Maximum number of records to return | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **offset** | **java.math.BigDecimal**| Number of records to skip | [optional] |

### Return type

[**ListProductsResponseDto**](ListProductsResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="updateProduct"></a>
# **updateProduct**
> kotlin.Any updateProduct(id, updateProductDto)

Update Product

Updates a product&#39;s name, description, or metadata.

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = ProductsApi()
val id : kotlin.String = id_example // kotlin.String | The unique identifier of the product
val updateProductDto : UpdateProductDto =  // UpdateProductDto | Product update details
try {
    val result : kotlin.Any = apiInstance.updateProduct(id, updateProductDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductsApi#updateProduct")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductsApi#updateProduct")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The unique identifier of the product | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateProductDto** | [**UpdateProductDto**](UpdateProductDto.md)| Product update details | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

