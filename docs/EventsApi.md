# EventsApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**listEvents**](EventsApi.md#listEvents) | **GET** /api/canary/events | List Events |


<a id="listEvents"></a>
# **listEvents**
> ListEventsResponseDto listEvents(merchantId, endDate, startDate, type, limit, offset)

List Events

Retrieves a log of all API events for debugging and logging.

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = EventsApi()
val merchantId : kotlin.String = merchantId_example // kotlin.String | The ID of the merchant. This parameter is required.
val endDate : kotlin.Any =  // kotlin.Any | Filter by end date
val startDate : kotlin.Any =  // kotlin.Any | Filter by start date
val type : kotlin.Any =  // kotlin.Any | Filter by event type
val limit : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Maximum number of records to return
val offset : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Number of records to skip
try {
    val result : ListEventsResponseDto = apiInstance.listEvents(merchantId, endDate, startDate, type, limit, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EventsApi#listEvents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EventsApi#listEvents")
    e.printStackTrace()
}
```

### Parameters
| **merchantId** | **kotlin.String**| The ID of the merchant. This parameter is required. | |
| **endDate** | [**kotlin.Any**](.md)| Filter by end date | [optional] |
| **startDate** | [**kotlin.Any**](.md)| Filter by start date | [optional] |
| **type** | [**kotlin.Any**](.md)| Filter by event type | [optional] |
| **limit** | **java.math.BigDecimal**| Maximum number of records to return | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **offset** | **java.math.BigDecimal**| Number of records to skip | [optional] |

### Return type

[**ListEventsResponseDto**](ListEventsResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

