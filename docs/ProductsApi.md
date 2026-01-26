# ProductsApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createProduct**](ProductsApi.md#createProduct) | **POST** /api/canary/products | Create Product |
| [**listProducts**](ProductsApi.md#listProducts) | **GET** /api/canary/products | List Products |
| [**retrieveMultipleProducts**](ProductsApi.md#retrieveMultipleProducts) | **POST** /api/canary/products/multiple | Retrieve Multiple Products by ID |
| [**retrieveProduct**](ProductsApi.md#retrieveProduct) | **GET** /api/canary/products/{id} | Retrieve Product |
| [**updateProduct**](ProductsApi.md#updateProduct) | **PATCH** /api/canary/products/{id} | Update Product |


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

<a id="listProducts"></a>
# **listProducts**
> ListProductsResponseDto listProducts(limit, offset, merchantId, active)

List Products

Retrieves all products in the merchant&#39;s catalog.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = ProductsApi()
val limit : java.math.BigDecimal = 50 // java.math.BigDecimal | Maximum number of records to return
val offset : java.math.BigDecimal = 0 // java.math.BigDecimal | Number of records to skip
val merchantId : kotlin.String = merchantId_example // kotlin.String | The ID of the merchant whose products are being requested. If not provided, the products of the authenticated merchant will be returned.
val active : kotlin.Boolean = true // kotlin.Boolean | Filter by active status
try {
    val result : ListProductsResponseDto = apiInstance.listProducts(limit, offset, merchantId, active)
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
| **limit** | **java.math.BigDecimal**| Maximum number of records to return | [optional] |
| **offset** | **java.math.BigDecimal**| Number of records to skip | [optional] |
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

<a id="retrieveMultipleProducts"></a>
# **retrieveMultipleProducts**
> kotlin.collections.List&lt;ProductResponseDto&gt; retrieveMultipleProducts(retrieveMultipleProductsDto)

Retrieve Multiple Products by ID

Retrieves multiple products using the provided ID&#39;s with a maximum of 50 IDs.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = ProductsApi()
val retrieveMultipleProductsDto : RetrieveMultipleProductsDto =  // RetrieveMultipleProductsDto | List of product IDs
try {
    val result : kotlin.collections.List<ProductResponseDto> = apiInstance.retrieveMultipleProducts(retrieveMultipleProductsDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductsApi#retrieveMultipleProducts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductsApi#retrieveMultipleProducts")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **retrieveMultipleProductsDto** | [**RetrieveMultipleProductsDto**](RetrieveMultipleProductsDto.md)| List of product IDs | |

### Return type

[**kotlin.collections.List&lt;ProductResponseDto&gt;**](ProductResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
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

