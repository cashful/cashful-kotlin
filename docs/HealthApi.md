# HealthApi

All URIs are relative to *http://localhost:9000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**checkHealth**](HealthApi.md#checkHealth) | **GET** /api/canary/health | Health check endpoint |


<a id="checkHealth"></a>
# **checkHealth**
> kotlin.Any checkHealth()

Health check endpoint

Performs a health check on the application and external dependencies

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = HealthApi()
try {
    val result : kotlin.Any = apiInstance.checkHealth()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HealthApi#checkHealth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HealthApi#checkHealth")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

