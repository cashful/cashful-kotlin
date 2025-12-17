# BalanceApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getBalanceHistory**](BalanceApi.md#getBalanceHistory) | **GET** /api/canary/balance/history | List Merchant Balance History |
| [**getMerchantBalance**](BalanceApi.md#getMerchantBalance) | **GET** /api/canary/balance | Get Merchant Balance |


<a id="getBalanceHistory"></a>
# **getBalanceHistory**
> BalanceHistoryResponseDto getBalanceHistory(merchantId, transactionType, endDate, startDate, limit, offset)

List Merchant Balance History

A full ledger of all transactions, fees, and payouts for the merchant&#39;s master account.

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = BalanceApi()
val merchantId : kotlin.String = merchantId_example // kotlin.String | The ID of the merchant. This parameter is required.
val transactionType : kotlin.Any =  // kotlin.Any | Filter by transaction type (e.g., \"credit\", \"debit\", \"fee\", \"payout\")
val endDate : kotlin.Any =  // kotlin.Any | Filter transactions until this date (ISO 8601 format)
val startDate : kotlin.Any =  // kotlin.Any | Filter transactions from this date (ISO 8601 format)
val limit : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Maximum number of records to return
val offset : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Number of records to skip
try {
    val result : BalanceHistoryResponseDto = apiInstance.getBalanceHistory(merchantId, transactionType, endDate, startDate, limit, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BalanceApi#getBalanceHistory")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BalanceApi#getBalanceHistory")
    e.printStackTrace()
}
```

### Parameters
| **merchantId** | **kotlin.String**| The ID of the merchant. This parameter is required. | |
| **transactionType** | [**kotlin.Any**](.md)| Filter by transaction type (e.g., \&quot;credit\&quot;, \&quot;debit\&quot;, \&quot;fee\&quot;, \&quot;payout\&quot;) | [optional] |
| **endDate** | [**kotlin.Any**](.md)| Filter transactions until this date (ISO 8601 format) | [optional] |
| **startDate** | [**kotlin.Any**](.md)| Filter transactions from this date (ISO 8601 format) | [optional] |
| **limit** | **java.math.BigDecimal**| Maximum number of records to return | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **offset** | **java.math.BigDecimal**| Number of records to skip | [optional] |

### Return type

[**BalanceHistoryResponseDto**](BalanceHistoryResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getMerchantBalance"></a>
# **getMerchantBalance**
> MerchantBalanceResponseDto getMerchantBalance(merchantId)

Get Merchant Balance

Retrieves the merchant&#39;s own master balance (their earnings) available for payouts.

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = BalanceApi()
val merchantId : kotlin.String = merchant_123 // kotlin.String | The unique identifier of the merchant
try {
    val result : MerchantBalanceResponseDto = apiInstance.getMerchantBalance(merchantId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BalanceApi#getMerchantBalance")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BalanceApi#getMerchantBalance")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **merchantId** | **kotlin.String**| The unique identifier of the merchant | |

### Return type

[**MerchantBalanceResponseDto**](MerchantBalanceResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

