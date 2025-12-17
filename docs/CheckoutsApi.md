# CheckoutsApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createCheckoutSession**](CheckoutsApi.md#createCheckoutSession) | **POST** /api/canary/checkout/sessions | Create Hosted Checkout |
| [**listAllCheckoutSessionsInternal**](CheckoutsApi.md#listAllCheckoutSessionsInternal) | **GET** /api/canary/checkout/sessions | List All Checkout Sessions |
| [**retrieveCheckoutSessionInternal**](CheckoutsApi.md#retrieveCheckoutSessionInternal) | **GET** /api/canary/checkout/sessions/{id} | Retrieve Checkout Session |


<a id="createCheckoutSession"></a>
# **createCheckoutSession**
> CheckoutSessionResponseDto createCheckoutSession(createCheckoutSessionDto)

Create Hosted Checkout

Creates a hosted payment page. Used for: (1) A standard e-commerce purchase, or (2) a \&quot;Pay-In\&quot; to fund a CustomerBalance.

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = CheckoutsApi()
val createCheckoutSessionDto : CreateCheckoutSessionDto =  // CreateCheckoutSessionDto | Checkout session details
try {
    val result : CheckoutSessionResponseDto = apiInstance.createCheckoutSession(createCheckoutSessionDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutsApi#createCheckoutSession")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutsApi#createCheckoutSession")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createCheckoutSessionDto** | [**CreateCheckoutSessionDto**](CreateCheckoutSessionDto.md)| Checkout session details | |

### Return type

[**CheckoutSessionResponseDto**](CheckoutSessionResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="listAllCheckoutSessionsInternal"></a>
# **listAllCheckoutSessionsInternal**
> kotlin.collections.List&lt;CheckoutSessionResponseDto&gt; listAllCheckoutSessionsInternal(merchantId, limit, offset)

List All Checkout Sessions

Lists all checkout sessions across all merchants (internal use only)

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = CheckoutsApi()
val merchantId : kotlin.String = merchantId_example // kotlin.String | The ID of the merchant. This parameter is required.
val limit : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Maximum number of records to return
val offset : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Number of records to skip
try {
    val result : kotlin.collections.List<CheckoutSessionResponseDto> = apiInstance.listAllCheckoutSessionsInternal(merchantId, limit, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutsApi#listAllCheckoutSessionsInternal")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutsApi#listAllCheckoutSessionsInternal")
    e.printStackTrace()
}
```

### Parameters
| **merchantId** | **kotlin.String**| The ID of the merchant. This parameter is required. | |
| **limit** | **java.math.BigDecimal**| Maximum number of records to return | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **offset** | **java.math.BigDecimal**| Number of records to skip | [optional] |

### Return type

[**kotlin.collections.List&lt;CheckoutSessionResponseDto&gt;**](CheckoutSessionResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="retrieveCheckoutSessionInternal"></a>
# **retrieveCheckoutSessionInternal**
> CheckoutSessionResponseDto retrieveCheckoutSessionInternal(id)

Retrieve Checkout Session

Retrieves details of a specific checkout session

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = CheckoutsApi()
val id : kotlin.String = id_example // kotlin.String | The unique identifier of the checkout session
try {
    val result : CheckoutSessionResponseDto = apiInstance.retrieveCheckoutSessionInternal(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutsApi#retrieveCheckoutSessionInternal")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutsApi#retrieveCheckoutSessionInternal")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique identifier of the checkout session | |

### Return type

[**CheckoutSessionResponseDto**](CheckoutSessionResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

