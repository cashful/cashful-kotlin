# CheckoutsApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createCheckoutSession**](CheckoutsApi.md#createCheckoutSession) | **POST** /api/canary/checkout/sessions | Create Hosted Checkout |
| [**listCheckoutSessions**](CheckoutsApi.md#listCheckoutSessions) | **GET** /api/canary/checkout/sessions | List Checkout Sessions |
| [**retrieveCheckoutSession**](CheckoutsApi.md#retrieveCheckoutSession) | **GET** /api/canary/checkout/sessions/{id} | Retrieve Checkout Session |


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

<a id="listCheckoutSessions"></a>
# **listCheckoutSessions**
> ListCheckoutSessionsResponseDto listCheckoutSessions(merchantId, limit, offset, status)

List Checkout Sessions

Lists checkout sessions

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = CheckoutsApi()
val merchantId : kotlin.String = merchantId_example // kotlin.String | The ID of the merchant. This parameter is required.
val limit : java.math.BigDecimal = 50 // java.math.BigDecimal | Maximum number of records to return
val offset : java.math.BigDecimal = 0 // java.math.BigDecimal | Number of records to skip
val status : kotlin.String = status_example // kotlin.String | The status to filter checkout sessions
try {
    val result : ListCheckoutSessionsResponseDto = apiInstance.listCheckoutSessions(merchantId, limit, offset, status)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutsApi#listCheckoutSessions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutsApi#listCheckoutSessions")
    e.printStackTrace()
}
```

### Parameters
| **merchantId** | **kotlin.String**| The ID of the merchant. This parameter is required. | |
| **limit** | **java.math.BigDecimal**| Maximum number of records to return | [optional] |
| **offset** | **java.math.BigDecimal**| Number of records to skip | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **status** | **kotlin.String**| The status to filter checkout sessions | [optional] |

### Return type

[**ListCheckoutSessionsResponseDto**](ListCheckoutSessionsResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="retrieveCheckoutSession"></a>
# **retrieveCheckoutSession**
> CheckoutSessionResponseDto retrieveCheckoutSession(id)

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
    val result : CheckoutSessionResponseDto = apiInstance.retrieveCheckoutSession(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutsApi#retrieveCheckoutSession")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutsApi#retrieveCheckoutSession")
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

