# PaymentIntentsApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cancelPaymentIntent**](PaymentIntentsApi.md#cancelPaymentIntent) | **POST** /api/canary/payment-intents/{id}/cancel | Cancel Payment Intent |
| [**confirmPaymentIntent**](PaymentIntentsApi.md#confirmPaymentIntent) | **POST** /api/canary/payment-intents/{id}/confirm | Confirm Payment Intent |
| [**createPaymentIntent**](PaymentIntentsApi.md#createPaymentIntent) | **POST** /api/canary/payment-intents | Create Payment Intent |
| [**listPaymentIntents**](PaymentIntentsApi.md#listPaymentIntents) | **GET** /api/canary/payment-intents | List Payment Intents |
| [**retrievePaymentIntent**](PaymentIntentsApi.md#retrievePaymentIntent) | **GET** /api/canary/payment-intents/{id} | Retrieve Payment Intent |


<a id="cancelPaymentIntent"></a>
# **cancelPaymentIntent**
> PaymentIntentResponseDto cancelPaymentIntent(id)

Cancel Payment Intent

Cancels a payment intent that has not yet succeeded or failed.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = PaymentIntentsApi()
val id : kotlin.String = id_example // kotlin.String | The unique identifier of the payment intent
try {
    val result : PaymentIntentResponseDto = apiInstance.cancelPaymentIntent(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentIntentsApi#cancelPaymentIntent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentIntentsApi#cancelPaymentIntent")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique identifier of the payment intent | |

### Return type

[**PaymentIntentResponseDto**](PaymentIntentResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="confirmPaymentIntent"></a>
# **confirmPaymentIntent**
> ConfirmPaymentIntentResponseDto confirmPaymentIntent(id, confirmPaymentIntentDto)

Confirm Payment Intent

Confirms a payment intent that requires confirmation and returns 3DS parameters for card authentication.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = PaymentIntentsApi()
val id : kotlin.String = id_example // kotlin.String | The unique identifier of the payment intent
val confirmPaymentIntentDto : ConfirmPaymentIntentDto =  // ConfirmPaymentIntentDto | 
try {
    val result : ConfirmPaymentIntentResponseDto = apiInstance.confirmPaymentIntent(id, confirmPaymentIntentDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentIntentsApi#confirmPaymentIntent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentIntentsApi#confirmPaymentIntent")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The unique identifier of the payment intent | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **confirmPaymentIntentDto** | [**ConfirmPaymentIntentDto**](ConfirmPaymentIntentDto.md)|  | |

### Return type

[**ConfirmPaymentIntentResponseDto**](ConfirmPaymentIntentResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="createPaymentIntent"></a>
# **createPaymentIntent**
> PaymentIntentResponseDto createPaymentIntent(createPaymentIntentDto)

Create Payment Intent

Creates a payment intent for a payment attempt. Used for hosted checkout or direct integrations.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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

<a id="listPaymentIntents"></a>
# **listPaymentIntents**
> ListPaymentIntentsResponseDto listPaymentIntents(status, offset, limit, merchantId)

List Payment Intents

Lists payment intents for a specific merchant with pagination and filtering.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = PaymentIntentsApi()
val status : kotlin.String = status_example // kotlin.String | 
val offset : java.math.BigDecimal = 8.14 // java.math.BigDecimal | 
val limit : java.math.BigDecimal = 8.14 // java.math.BigDecimal | 
val merchantId : kotlin.String = merchantId_example // kotlin.String | 
try {
    val result : ListPaymentIntentsResponseDto = apiInstance.listPaymentIntents(status, offset, limit, merchantId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentIntentsApi#listPaymentIntents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentIntentsApi#listPaymentIntents")
    e.printStackTrace()
}
```

### Parameters
| **status** | **kotlin.String**|  | [optional] [enum: initiation, requires_payment_method, requires_confirmation, requires_action, processing, requires_capture, succeeded, failed, canceled] |
| **offset** | **java.math.BigDecimal**|  | [optional] |
| **limit** | **java.math.BigDecimal**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **merchantId** | **kotlin.String**|  | [optional] |

### Return type

[**ListPaymentIntentsResponseDto**](ListPaymentIntentsResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="retrievePaymentIntent"></a>
# **retrievePaymentIntent**
> PaymentIntentResponseDto retrievePaymentIntent(id)

Retrieve Payment Intent

Retrieves the current state of a specific payment intent.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = PaymentIntentsApi()
val id : kotlin.String = id_example // kotlin.String | The unique identifier of the payment intent
try {
    val result : PaymentIntentResponseDto = apiInstance.retrievePaymentIntent(id)
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

[**PaymentIntentResponseDto**](PaymentIntentResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

