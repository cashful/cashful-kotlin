# CheckoutsApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createCheckoutSession**](CheckoutsApi.md#createCheckoutSession) | **POST** /api/canary/checkout/sessions | Create Hosted Checkout |


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

