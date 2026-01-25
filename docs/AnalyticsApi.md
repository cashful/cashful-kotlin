# AnalyticsApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getAnalytics**](AnalyticsApi.md#getAnalytics) | **GET** /api/canary/analytics | Get Analytics |
| [**getAnalyticsSummary**](AnalyticsApi.md#getAnalyticsSummary) | **GET** /api/canary/analytics/summary | Get Analytics Summary |


<a id="getAnalytics"></a>
# **getAnalytics**
> AnalyticsResponseDto getAnalytics(merchantId)

Get Analytics

Retrieves transaction volume and customer growth metrics for the merchant.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AnalyticsApi()
val merchantId : kotlin.String = merchant_123 // kotlin.String | The unique identifier of the merchant. If not provided, defaults to the authenticated user's active organization.
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
| **merchantId** | **kotlin.String**| The unique identifier of the merchant. If not provided, defaults to the authenticated user&#39;s active organization. | [optional] |

### Return type

[**AnalyticsResponseDto**](AnalyticsResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getAnalyticsSummary"></a>
# **getAnalyticsSummary**
> AnalyticsSummaryDto getAnalyticsSummary(merchantId)

Get Analytics Summary

Retrieves a quick summary of key metrics for the merchant.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AnalyticsApi()
val merchantId : kotlin.String = merchant_123 // kotlin.String | The unique identifier of the merchant. If not provided, defaults to the authenticated user's active organization.
try {
    val result : AnalyticsSummaryDto = apiInstance.getAnalyticsSummary(merchantId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AnalyticsApi#getAnalyticsSummary")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AnalyticsApi#getAnalyticsSummary")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **merchantId** | **kotlin.String**| The unique identifier of the merchant. If not provided, defaults to the authenticated user&#39;s active organization. | [optional] |

### Return type

[**AnalyticsSummaryDto**](AnalyticsSummaryDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

