# BalanceApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getBalanceHistory**](BalanceApi.md#getBalanceHistory) | **GET** /api/canary/balance/history | List Merchant Balance History |
| [**getMerchantBalance**](BalanceApi.md#getMerchantBalance) | **GET** /api/canary/balance | Get Merchant Balance |


<a id="getBalanceHistory"></a>
# **getBalanceHistory**
> BalanceHistoryResponseDto getBalanceHistory(limit, offset, filter, sort, order, merchantId, startDate, endDate, transactionType)

List Merchant Balance History

A full ledger of all transactions, fees, and payouts for the merchant&#39;s master account.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = BalanceApi()
val limit : java.math.BigDecimal = 50 // java.math.BigDecimal | Maximum number of items to return
val offset : java.math.BigDecimal = 0 // java.math.BigDecimal | Number of items to skip
val filter : kotlin.String = {"ids":["prod_123","prod_456"]} // kotlin.String | JSON string used for dynamic filtering
val sort : kotlin.String = createdAt // kotlin.String | Field name to sort by
val order : kotlin.String = DESC // kotlin.String | Sort direction
val merchantId : kotlin.String = merchantId_example // kotlin.String | The ID of the merchant whose balance is being requested. If omitted, defaults to the authenticated merchant.
val startDate : kotlin.String = startDate_example // kotlin.String | Filter transactions from this date (ISO 8601 format)
val endDate : kotlin.String = endDate_example // kotlin.String | Filter transactions until this date (ISO 8601 format)
val transactionType : kotlin.String = transactionType_example // kotlin.String | Filter by transaction type (e.g., \"credit\", \"debit\", \"fee\", \"payout\")
try {
    val result : BalanceHistoryResponseDto = apiInstance.getBalanceHistory(limit, offset, filter, sort, order, merchantId, startDate, endDate, transactionType)
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
| **limit** | **java.math.BigDecimal**| Maximum number of items to return | [optional] |
| **offset** | **java.math.BigDecimal**| Number of items to skip | [optional] |
| **filter** | **kotlin.String**| JSON string used for dynamic filtering | [optional] |
| **sort** | **kotlin.String**| Field name to sort by | [optional] |
| **order** | **kotlin.String**| Sort direction | [optional] |
| **merchantId** | **kotlin.String**| The ID of the merchant whose balance is being requested. If omitted, defaults to the authenticated merchant. | [optional] |
| **startDate** | **kotlin.String**| Filter transactions from this date (ISO 8601 format) | [optional] |
| **endDate** | **kotlin.String**| Filter transactions until this date (ISO 8601 format) | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **transactionType** | **kotlin.String**| Filter by transaction type (e.g., \&quot;credit\&quot;, \&quot;debit\&quot;, \&quot;fee\&quot;, \&quot;payout\&quot;) | [optional] |

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = BalanceApi()
val merchantId : kotlin.String = merchantId_example // kotlin.String | The ID of the merchant whose balance is being requested. If omitted, defaults to the authenticated merchant.
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
| **merchantId** | **kotlin.String**| The ID of the merchant whose balance is being requested. If omitted, defaults to the authenticated merchant. | [optional] |

### Return type

[**MerchantBalanceResponseDto**](MerchantBalanceResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

