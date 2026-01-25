# EventsApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**listEvents**](EventsApi.md#listEvents) | **GET** /api/canary/events | List Events |


<a id="listEvents"></a>
# **listEvents**
> ListEventsResponseDto listEvents(merchantId, limit, offset, type, status, startDate, endDate)

List Events

Retrieves a log of all API events for debugging and logging.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = EventsApi()
val merchantId : kotlin.String = merchantId_example // kotlin.String | The ID of the merchant whose events are being requested. This parameter is required.
val limit : java.math.BigDecimal = 50 // java.math.BigDecimal | Maximum number of records to return
val offset : java.math.BigDecimal = 0 // java.math.BigDecimal | Number of records to skip
val type : kotlin.String = type_example // kotlin.String | Filter by event type
val status : kotlin.String = status_example // kotlin.String | Filter by event status
val startDate : kotlin.String = startDate_example // kotlin.String | Filter by start date
val endDate : kotlin.String = endDate_example // kotlin.String | Filter by end date
try {
    val result : ListEventsResponseDto = apiInstance.listEvents(merchantId, limit, offset, type, status, startDate, endDate)
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
| **merchantId** | **kotlin.String**| The ID of the merchant whose events are being requested. This parameter is required. | |
| **limit** | **java.math.BigDecimal**| Maximum number of records to return | [optional] |
| **offset** | **java.math.BigDecimal**| Number of records to skip | [optional] |
| **type** | **kotlin.String**| Filter by event type | [optional] |
| **status** | **kotlin.String**| Filter by event status | [optional] [enum: pending, delivered, failed] |
| **startDate** | **kotlin.String**| Filter by start date | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **endDate** | **kotlin.String**| Filter by end date | [optional] |

### Return type

[**ListEventsResponseDto**](ListEventsResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

