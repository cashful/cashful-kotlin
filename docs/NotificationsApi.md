# NotificationsApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**sendEmail**](NotificationsApi.md#sendEmail) | **POST** /api/canary/notifications/email | Send an email notification |
| [**sendMultiChannelNotification**](NotificationsApi.md#sendMultiChannelNotification) | **POST** /api/canary/notifications/multi-channel | Send notifications via multiple channels |
| [**sendNotification**](NotificationsApi.md#sendNotification) | **POST** /api/canary/notifications/send | Send a notification via specified channel |
| [**sendSms**](NotificationsApi.md#sendSms) | **POST** /api/canary/notifications/sms | Send an SMS notification |


<a id="sendEmail"></a>
# **sendEmail**
> SendEmail200Response sendEmail(sendEmailDto)

Send an email notification

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = NotificationsApi()
val sendEmailDto : SendEmailDto =  // SendEmailDto | 
try {
    val result : SendEmail200Response = apiInstance.sendEmail(sendEmailDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NotificationsApi#sendEmail")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NotificationsApi#sendEmail")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sendEmailDto** | [**SendEmailDto**](SendEmailDto.md)|  | |

### Return type

[**SendEmail200Response**](SendEmail200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="sendMultiChannelNotification"></a>
# **sendMultiChannelNotification**
> SendMultiChannelNotification200Response sendMultiChannelNotification()

Send notifications via multiple channels

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = NotificationsApi()
try {
    val result : SendMultiChannelNotification200Response = apiInstance.sendMultiChannelNotification()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NotificationsApi#sendMultiChannelNotification")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NotificationsApi#sendMultiChannelNotification")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**SendMultiChannelNotification200Response**](SendMultiChannelNotification200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="sendNotification"></a>
# **sendNotification**
> sendNotification(notificationDto)

Send a notification via specified channel

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = NotificationsApi()
val notificationDto : NotificationDto =  // NotificationDto | 
try {
    apiInstance.sendNotification(notificationDto)
} catch (e: ClientException) {
    println("4xx response calling NotificationsApi#sendNotification")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NotificationsApi#sendNotification")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **notificationDto** | [**NotificationDto**](NotificationDto.md)|  | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="sendSms"></a>
# **sendSms**
> SendSms200Response sendSms(sendSmsDto)

Send an SMS notification

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = NotificationsApi()
val sendSmsDto : SendSmsDto =  // SendSmsDto | 
try {
    val result : SendSms200Response = apiInstance.sendSms(sendSmsDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NotificationsApi#sendSms")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NotificationsApi#sendSms")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sendSmsDto** | [**SendSmsDto**](SendSmsDto.md)|  | |

### Return type

[**SendSms200Response**](SendSms200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

