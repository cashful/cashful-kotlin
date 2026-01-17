# WebhooksApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createWebhookEndpoint**](WebhooksApi.md#createWebhookEndpoint) | **POST** /api/canary/webhook-endpoints | Create Webhook Endpoint |
| [**deleteWebhookEndpoint**](WebhooksApi.md#deleteWebhookEndpoint) | **DELETE** /api/canary/webhook-endpoints/{id} | Delete Webhook Endpoint |
| [**listWebhookEndpoints**](WebhooksApi.md#listWebhookEndpoints) | **GET** /api/canary/webhook-endpoints | List Webhook Endpoints |


<a id="createWebhookEndpoint"></a>
# **createWebhookEndpoint**
> WebhookEndpointResponseDto createWebhookEndpoint(createWebhookEndpointDto)

Create Webhook Endpoint

Registers a URL to receive real-time events (e.g., checkout.session.completed, purchase.succeeded).

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = WebhooksApi()
val createWebhookEndpointDto : CreateWebhookEndpointDto =  // CreateWebhookEndpointDto | Webhook endpoint details
try {
    val result : WebhookEndpointResponseDto = apiInstance.createWebhookEndpoint(createWebhookEndpointDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#createWebhookEndpoint")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#createWebhookEndpoint")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createWebhookEndpointDto** | [**CreateWebhookEndpointDto**](CreateWebhookEndpointDto.md)| Webhook endpoint details | |

### Return type

[**WebhookEndpointResponseDto**](WebhookEndpointResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="deleteWebhookEndpoint"></a>
# **deleteWebhookEndpoint**
> kotlin.Any deleteWebhookEndpoint(id)

Delete Webhook Endpoint

Stops sending events to a specific URL.

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = WebhooksApi()
val id : kotlin.String = id_example // kotlin.String | The unique identifier of the webhook endpoint
try {
    val result : kotlin.Any = apiInstance.deleteWebhookEndpoint(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#deleteWebhookEndpoint")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#deleteWebhookEndpoint")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique identifier of the webhook endpoint | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listWebhookEndpoints"></a>
# **listWebhookEndpoints**
> ListWebhookEndpointsResponseDto listWebhookEndpoints(merchantId, limit, offset)

List Webhook Endpoints

Lists all configured webhook endpoints.

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = WebhooksApi()
val merchantId : kotlin.String = merchantId_example // kotlin.String | The ID of the merchant. This parameter is required.
val limit : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Maximum number of records to return
val offset : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Number of records to skip
try {
    val result : ListWebhookEndpointsResponseDto = apiInstance.listWebhookEndpoints(merchantId, limit, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#listWebhookEndpoints")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#listWebhookEndpoints")
    e.printStackTrace()
}
```

### Parameters
| **merchantId** | **kotlin.String**| The ID of the merchant. This parameter is required. | |
| **limit** | **java.math.BigDecimal**| Maximum number of records to return | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **offset** | **java.math.BigDecimal**| Number of records to skip | [optional] |

### Return type

[**ListWebhookEndpointsResponseDto**](ListWebhookEndpointsResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

