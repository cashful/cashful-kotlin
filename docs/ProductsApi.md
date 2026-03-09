# ProductsApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createProduct**](ProductsApi.md#createProduct) | **POST** /api/canary/products | Create Product |
| [**deleteProduct**](ProductsApi.md#deleteProduct) | **DELETE** /api/canary/products/{id} | Delete Product |
| [**deleteProductsBulk**](ProductsApi.md#deleteProductsBulk) | **DELETE** /api/canary/products/bulk | Bulk Delete Products |
| [**listProducts**](ProductsApi.md#listProducts) | **GET** /api/canary/products | List Products |
| [**retrieveProduct**](ProductsApi.md#retrieveProduct) | **GET** /api/canary/products/{id} | Retrieve Product |
| [**updateProduct**](ProductsApi.md#updateProduct) | **PATCH** /api/canary/products/{id} | Update Product |
| [**updateProductsBulk**](ProductsApi.md#updateProductsBulk) | **PATCH** /api/canary/products/bulk | Bulk Update Products |


<a id="createProduct"></a>
# **createProduct**
> ProductResponseDto createProduct(createProductDto)

Create Product

Defines a product in the merchant&#39;s catalog (e.g., \&quot;Airtime,\&quot; \&quot;Data\&quot;).

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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

<a id="deleteProduct"></a>
# **deleteProduct**
> ProductResponseDto deleteProduct(id)

Delete Product

Deletes a product by ID.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = ProductsApi()
val id : kotlin.String = id_example // kotlin.String | The unique identifier of the product
try {
    val result : ProductResponseDto = apiInstance.deleteProduct(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductsApi#deleteProduct")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductsApi#deleteProduct")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique identifier of the product | |

### Return type

[**ProductResponseDto**](ProductResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="deleteProductsBulk"></a>
# **deleteProductsBulk**
> kotlin.Any deleteProductsBulk(bulkIdsDto)

Bulk Delete Products

Deletes multiple products by ID.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = ProductsApi()
val bulkIdsDto : BulkIdsDto =  // BulkIdsDto | 
try {
    val result : kotlin.Any = apiInstance.deleteProductsBulk(bulkIdsDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductsApi#deleteProductsBulk")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductsApi#deleteProductsBulk")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **bulkIdsDto** | [**BulkIdsDto**](BulkIdsDto.md)|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="listProducts"></a>
# **listProducts**
> ListProductsResponseDto listProducts(limit, offset, filter, sort, order, merchantId, active)

List Products

Retrieves all products in the merchant&#39;s catalog.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = ProductsApi()
val limit : java.math.BigDecimal = 50 // java.math.BigDecimal | Maximum number of items to return
val offset : java.math.BigDecimal = 0 // java.math.BigDecimal | Number of items to skip
val filter : kotlin.String = {"ids":["prod_123","prod_456"]} // kotlin.String | JSON string used for dynamic filtering
val sort : kotlin.String = createdAt // kotlin.String | Field name to sort by
val order : kotlin.String = DESC // kotlin.String | Sort direction
val merchantId : kotlin.String = merchantId_example // kotlin.String | The ID of the merchant whose products are being requested. If not provided, the products of the authenticated merchant will be returned.
val active : kotlin.Boolean = true // kotlin.Boolean | Filter by active status
try {
    val result : ListProductsResponseDto = apiInstance.listProducts(limit, offset, filter, sort, order, merchantId, active)
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
| **limit** | **java.math.BigDecimal**| Maximum number of items to return | [optional] |
| **offset** | **java.math.BigDecimal**| Number of items to skip | [optional] |
| **filter** | **kotlin.String**| JSON string used for dynamic filtering | [optional] |
| **sort** | **kotlin.String**| Field name to sort by | [optional] [enum: id, name, amount, currency, active, merchantId, createdAt, updatedAt] |
| **order** | **kotlin.String**| Sort direction | [optional] |
| **merchantId** | **kotlin.String**| The ID of the merchant whose products are being requested. If not provided, the products of the authenticated merchant will be returned. | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **active** | **kotlin.Boolean**| Filter by active status | [optional] |

### Return type

[**ListProductsResponseDto**](ListProductsResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="retrieveProduct"></a>
# **retrieveProduct**
> ProductResponseDto retrieveProduct(id)

Retrieve Product

Retrieves a single product by ID.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = ProductsApi()
val id : kotlin.String = id_example // kotlin.String | The unique identifier of the product
try {
    val result : ProductResponseDto = apiInstance.retrieveProduct(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductsApi#retrieveProduct")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductsApi#retrieveProduct")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique identifier of the product | |

### Return type

[**ProductResponseDto**](ProductResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="updateProduct"></a>
# **updateProduct**
> ProductResponseDto updateProduct(id, updateProductDto)

Update Product

Updates a product&#39;s name, description, or metadata.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = ProductsApi()
val id : kotlin.String = id_example // kotlin.String | The unique identifier of the product
val updateProductDto : UpdateProductDto =  // UpdateProductDto | Product update details
try {
    val result : ProductResponseDto = apiInstance.updateProduct(id, updateProductDto)
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

[**ProductResponseDto**](ProductResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="updateProductsBulk"></a>
# **updateProductsBulk**
> kotlin.Any updateProductsBulk(bulkUpdateProductsInputDto)

Bulk Update Products

Updates multiple products using a shared patch.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = ProductsApi()
val bulkUpdateProductsInputDto : BulkUpdateProductsInputDto =  // BulkUpdateProductsInputDto | 
try {
    val result : kotlin.Any = apiInstance.updateProductsBulk(bulkUpdateProductsInputDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductsApi#updateProductsBulk")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductsApi#updateProductsBulk")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **bulkUpdateProductsInputDto** | [**BulkUpdateProductsInputDto**](BulkUpdateProductsInputDto.md)|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

