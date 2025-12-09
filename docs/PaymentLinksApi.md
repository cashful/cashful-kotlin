# PaymentLinksApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createPaymentLink**](PaymentLinksApi.md#createPaymentLink) | **POST** /api/canary/payment-links | Create Payment Link |
| [**listPaymentLinks**](PaymentLinksApi.md#listPaymentLinks) | **GET** /api/canary/payment-links | List Payment Links |
| [**updatePaymentLink**](PaymentLinksApi.md#updatePaymentLink) | **PATCH** /api/canary/payment-links/{id} | Update Payment Link |


<a id="createPaymentLink"></a>
# **createPaymentLink**
> PaymentLinkResponseDto createPaymentLink(createPaymentLinkDto)

Create Payment Link

Creates a re-usable hosted link. Can be used for: (1) Selling a product, or (2) as a \&quot;Pay-In\&quot; link for a customer.

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = PaymentLinksApi()
val createPaymentLinkDto : CreatePaymentLinkDto =  // CreatePaymentLinkDto | Payment link details
try {
    val result : PaymentLinkResponseDto = apiInstance.createPaymentLink(createPaymentLinkDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentLinksApi#createPaymentLink")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentLinksApi#createPaymentLink")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createPaymentLinkDto** | [**CreatePaymentLinkDto**](CreatePaymentLinkDto.md)| Payment link details | |

### Return type

[**PaymentLinkResponseDto**](PaymentLinkResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="listPaymentLinks"></a>
# **listPaymentLinks**
> ListPaymentLinksResponseDto listPaymentLinks(merchantId, active, limit, offset)

List Payment Links

Retrieves all payment links created by the merchant.

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = PaymentLinksApi()
val merchantId : kotlin.String = merchantId_example // kotlin.String | The ID of the merchant. This parameter is required.
val active : kotlin.Boolean = true // kotlin.Boolean | Filter by active status
val limit : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Maximum number of records to return
val offset : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Number of records to skip
try {
    val result : ListPaymentLinksResponseDto = apiInstance.listPaymentLinks(merchantId, active, limit, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentLinksApi#listPaymentLinks")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentLinksApi#listPaymentLinks")
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

[**ListPaymentLinksResponseDto**](ListPaymentLinksResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="updatePaymentLink"></a>
# **updatePaymentLink**
> kotlin.Any updatePaymentLink(id, updatePaymentLinkDto)

Update Payment Link

Updates a link&#39;s details, most commonly to set active: false.

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = PaymentLinksApi()
val id : kotlin.String = id_example // kotlin.String | The unique identifier of the payment link
val updatePaymentLinkDto : UpdatePaymentLinkDto =  // UpdatePaymentLinkDto | Payment link update details
try {
    val result : kotlin.Any = apiInstance.updatePaymentLink(id, updatePaymentLinkDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentLinksApi#updatePaymentLink")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentLinksApi#updatePaymentLink")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The unique identifier of the payment link | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updatePaymentLinkDto** | [**UpdatePaymentLinkDto**](UpdatePaymentLinkDto.md)| Payment link update details | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

