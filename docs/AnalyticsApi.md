# AnalyticsApi

All URIs are relative to *http://localhost:9000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getAnalytics**](AnalyticsApi.md#getAnalytics) | **GET** /api/canary/analytics | Get Analytics |


<a id="getAnalytics"></a>
# **getAnalytics**
> AnalyticsResponseDto getAnalytics(merchantId)

Get Analytics

Retrieves transaction volume and customer growth metrics for the merchant.

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AnalyticsApi()
val merchantId : kotlin.String = merchant_123 // kotlin.String | The unique identifier of the merchant
try {
    val result : AnalyticsResponseDto = apiInstance.getAnalytics(merchantId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AnalyticsApi#getAnalytics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AnalyticsApi#getAnalytics")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **merchantId** | **kotlin.String**| The unique identifier of the merchant | |

### Return type

[**AnalyticsResponseDto**](AnalyticsResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

