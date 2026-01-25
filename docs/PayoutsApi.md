# PayoutsApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createPayout**](PayoutsApi.md#createPayout) | **POST** /api/canary/payouts | Create Payout |
| [**listPayouts**](PayoutsApi.md#listPayouts) | **GET** /api/canary/payouts | List Payouts |


<a id="createPayout"></a>
# **createPayout**
> PayoutResponseDto createPayout(createPayoutDto)

Create Payout

Allows the merchant to move funds from their MerchantBalance (their earnings) to their external bank account.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = PayoutsApi()
val createPayoutDto : CreatePayoutDto =  // CreatePayoutDto | Payout details
try {
    val result : PayoutResponseDto = apiInstance.createPayout(createPayoutDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PayoutsApi#createPayout")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayoutsApi#createPayout")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createPayoutDto** | [**CreatePayoutDto**](CreatePayoutDto.md)| Payout details | |

### Return type

[**PayoutResponseDto**](PayoutResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="listPayouts"></a>
# **listPayouts**
> ListPayoutsResponseDto listPayouts(merchantId, limit, offset, status)

List Payouts

Retrieves a list of all historical and pending payouts for the merchant.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = PayoutsApi()
val merchantId : kotlin.String = merchantId_example // kotlin.String | The ID of the merchant whose payouts are being requested. If omitted, defaults to the authenticated merchant.
val limit : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Maximum number of records to return
val offset : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Number of records to skip
val status : kotlin.String = status_example // kotlin.String | Filter by status
try {
    val result : ListPayoutsResponseDto = apiInstance.listPayouts(merchantId, limit, offset, status)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PayoutsApi#listPayouts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayoutsApi#listPayouts")
    e.printStackTrace()
}
```

### Parameters
| **merchantId** | **kotlin.String**| The ID of the merchant whose payouts are being requested. If omitted, defaults to the authenticated merchant. | [optional] |
| **limit** | **java.math.BigDecimal**| Maximum number of records to return | [optional] |
| **offset** | **java.math.BigDecimal**| Number of records to skip | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **status** | **kotlin.String**| Filter by status | [optional] |

### Return type

[**ListPayoutsResponseDto**](ListPayoutsResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

