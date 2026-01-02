# PaymentIntentsApi

All URIs are relative to *http://localhost:9000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createPaymentIntent**](PaymentIntentsApi.md#createPaymentIntent) | **POST** /api/canary/payment-intents | Create Off-Session Charge |
| [**retrievePaymentIntent**](PaymentIntentsApi.md#retrievePaymentIntent) | **GET** /api/canary/payment-intents/{id} | Retrieve Payment Intent |


<a id="createPaymentIntent"></a>
# **createPaymentIntent**
> PaymentIntentResponseDto createPaymentIntent(createPaymentIntentDto)

Create Off-Session Charge

Server-to-server API to charge a saved card. Used for subscriptions or recurring billing (a core gateway feature).

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = PaymentIntentsApi()
val createPaymentIntentDto : CreatePaymentIntentDto =  // CreatePaymentIntentDto | Payment intent details
try {
    val result : PaymentIntentResponseDto = apiInstance.createPaymentIntent(createPaymentIntentDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentIntentsApi#createPaymentIntent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentIntentsApi#createPaymentIntent")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createPaymentIntentDto** | [**CreatePaymentIntentDto**](CreatePaymentIntentDto.md)| Payment intent details | |

### Return type

[**PaymentIntentResponseDto**](PaymentIntentResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="retrievePaymentIntent"></a>
# **retrievePaymentIntent**
> kotlin.Any retrievePaymentIntent(id)

Retrieve Payment Intent

Checks the status of a specific server-to-server charge.

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = PaymentIntentsApi()
val id : kotlin.String = id_example // kotlin.String | The unique identifier of the payment intent
try {
    val result : kotlin.Any = apiInstance.retrievePaymentIntent(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentIntentsApi#retrievePaymentIntent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentIntentsApi#retrievePaymentIntent")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique identifier of the payment intent | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

