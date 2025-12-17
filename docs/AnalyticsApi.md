# AnalyticsApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getAnalytics**](AnalyticsApi.md#getAnalytics) | **GET** /api/canary/analytics | Get Analytics |


<a id="getAnalytics"></a>
# **getAnalytics**
> AnalyticsResponseDto getAnalytics()

Get Analytics

Retrieves transaction volume and customer growth metrics for the merchant.

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AnalyticsApi()
try {
    val result : AnalyticsResponseDto = apiInstance.getAnalytics()
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
This endpoint does not need any parameter.

### Return type

[**AnalyticsResponseDto**](AnalyticsResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

