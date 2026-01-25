# PaymentMethodsApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**deletePaymentMethod**](PaymentMethodsApi.md#deletePaymentMethod) | **DELETE** /api/canary/payment-methods/{id} | Delete Payment Method |
| [**listPaymentMethods**](PaymentMethodsApi.md#listPaymentMethods) | **GET** /api/canary/payment-methods | List Payment Methods |
| [**retrievePaymentMethod**](PaymentMethodsApi.md#retrievePaymentMethod) | **GET** /api/canary/payment-methods/{id} | Retrieve Payment Method |


<a id="deletePaymentMethod"></a>
# **deletePaymentMethod**
> kotlin.Any deletePaymentMethod(id)

Delete Payment Method

Detaches and deletes a saved payment method from a customer.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = PaymentMethodsApi()
val id : kotlin.String = id_example // kotlin.String | The unique identifier of the payment method
try {
    val result : kotlin.Any = apiInstance.deletePaymentMethod(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentMethodsApi#deletePaymentMethod")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentMethodsApi#deletePaymentMethod")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique identifier of the payment method | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listPaymentMethods"></a>
# **listPaymentMethods**
> ListPaymentMethodsResponseDto listPaymentMethods(limit, offset, merchantId, customerId)

List Payment Methods

Lists saved payment methods for a specific customer.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = PaymentMethodsApi()
val limit : java.math.BigDecimal = 50 // java.math.BigDecimal | Maximum number of records to return
val offset : java.math.BigDecimal = 0 // java.math.BigDecimal | Number of records to skip
val merchantId : kotlin.String = merchantId_example // kotlin.String | The unique identifier of the merchant. If not provided, defaults to the authenticated user's active organization.
val customerId : kotlin.String = customerId_example // kotlin.String | The unique identifier of the customer
try {
    val result : ListPaymentMethodsResponseDto = apiInstance.listPaymentMethods(limit, offset, merchantId, customerId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentMethodsApi#listPaymentMethods")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentMethodsApi#listPaymentMethods")
    e.printStackTrace()
}
```

### Parameters
| **limit** | **java.math.BigDecimal**| Maximum number of records to return | [optional] |
| **offset** | **java.math.BigDecimal**| Number of records to skip | [optional] |
| **merchantId** | **kotlin.String**| The unique identifier of the merchant. If not provided, defaults to the authenticated user&#39;s active organization. | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **customerId** | **kotlin.String**| The unique identifier of the customer | [optional] |

### Return type

[**ListPaymentMethodsResponseDto**](ListPaymentMethodsResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="retrievePaymentMethod"></a>
# **retrievePaymentMethod**
> PaymentMethodResponseDto retrievePaymentMethod(id)

Retrieve Payment Method

Gets the non-sensitive details of a saved card (e.g., brand, last 4).

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = PaymentMethodsApi()
val id : kotlin.String = id_example // kotlin.String | The unique identifier of the payment method
try {
    val result : PaymentMethodResponseDto = apiInstance.retrievePaymentMethod(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentMethodsApi#retrievePaymentMethod")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentMethodsApi#retrievePaymentMethod")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique identifier of the payment method | |

### Return type

[**PaymentMethodResponseDto**](PaymentMethodResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

