# StorageApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**storageControllerConfirmUploadCanary**](StorageApi.md#storageControllerConfirmUploadCanary) | **POST** /api/canary/storage/confirm-upload | Confirm that a file upload was completed |
| [**storageControllerDeleteCanary**](StorageApi.md#storageControllerDeleteCanary) | **DELETE** /api/canary/storage/{id} | Delete a file |
| [**storageControllerGetDownloadUrlCanary**](StorageApi.md#storageControllerGetDownloadUrlCanary) | **GET** /api/canary/storage/{id}/download-url | Get a presigned download URL for a file |
| [**storageControllerListCanary**](StorageApi.md#storageControllerListCanary) | **GET** /api/canary/storage | List files |
| [**storageControllerRequestUploadUrlCanary**](StorageApi.md#storageControllerRequestUploadUrlCanary) | **POST** /api/canary/storage/upload-url | Request a presigned URL for file upload |
| [**storageControllerRetrieveCanary**](StorageApi.md#storageControllerRetrieveCanary) | **GET** /api/canary/storage/{id} | Get file details |


<a id="storageControllerConfirmUploadCanary"></a>
# **storageControllerConfirmUploadCanary**
> FileDto storageControllerConfirmUploadCanary(confirmUploadDto)

Confirm that a file upload was completed

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = StorageApi()
val confirmUploadDto : ConfirmUploadDto = {"fileId":"file_abc123xyz","checksum":"sha256:a1b2c3d4e5f6...","size":245760} // ConfirmUploadDto | 
try {
    val result : FileDto = apiInstance.storageControllerConfirmUploadCanary(confirmUploadDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StorageApi#storageControllerConfirmUploadCanary")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StorageApi#storageControllerConfirmUploadCanary")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **confirmUploadDto** | [**ConfirmUploadDto**](ConfirmUploadDto.md)|  | |

### Return type

[**FileDto**](FileDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="storageControllerDeleteCanary"></a>
# **storageControllerDeleteCanary**
> storageControllerDeleteCanary(id)

Delete a file

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = StorageApi()
val id : kotlin.String = id_example // kotlin.String | File ID
try {
    apiInstance.storageControllerDeleteCanary(id)
} catch (e: ClientException) {
    println("4xx response calling StorageApi#storageControllerDeleteCanary")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StorageApi#storageControllerDeleteCanary")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| File ID | |

### Return type

null (empty response body)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="storageControllerGetDownloadUrlCanary"></a>
# **storageControllerGetDownloadUrlCanary**
> PresignedDownloadResponseDto storageControllerGetDownloadUrlCanary(id)

Get a presigned download URL for a file

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = StorageApi()
val id : kotlin.String = id_example // kotlin.String | File ID
try {
    val result : PresignedDownloadResponseDto = apiInstance.storageControllerGetDownloadUrlCanary(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StorageApi#storageControllerGetDownloadUrlCanary")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StorageApi#storageControllerGetDownloadUrlCanary")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| File ID | |

### Return type

[**PresignedDownloadResponseDto**](PresignedDownloadResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="storageControllerListCanary"></a>
# **storageControllerListCanary**
> ListFilesResponseDto storageControllerListCanary(merchantId, limit, offset, tag, status, relatedEntityId, relatedEntityType)

List files

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = StorageApi()
val merchantId : kotlin.String = merchantId_example // kotlin.String | The ID of the merchant. This parameter is required.
val limit : java.math.BigDecimal = 50 // java.math.BigDecimal | Maximum number of records to return
val offset : java.math.BigDecimal = 0 // java.math.BigDecimal | Number of records to skip
val tag : kotlin.String = tag_example // kotlin.String | Filter by tag
val status : kotlin.String = status_example // kotlin.String | 
val relatedEntityId : kotlin.String = relatedEntityId_example // kotlin.String | 
val relatedEntityType : kotlin.String = relatedEntityType_example // kotlin.String | 
try {
    val result : ListFilesResponseDto = apiInstance.storageControllerListCanary(merchantId, limit, offset, tag, status, relatedEntityId, relatedEntityType)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StorageApi#storageControllerListCanary")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StorageApi#storageControllerListCanary")
    e.printStackTrace()
}
```

### Parameters
| **merchantId** | **kotlin.String**| The ID of the merchant. This parameter is required. | |
| **limit** | **java.math.BigDecimal**| Maximum number of records to return | [optional] |
| **offset** | **java.math.BigDecimal**| Number of records to skip | [optional] |
| **tag** | **kotlin.String**| Filter by tag | [optional] |
| **status** | **kotlin.String**|  | [optional] [enum: pending, uploaded, failed, deleted] |
| **relatedEntityId** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **relatedEntityType** | **kotlin.String**|  | [optional] |

### Return type

[**ListFilesResponseDto**](ListFilesResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="storageControllerRequestUploadUrlCanary"></a>
# **storageControllerRequestUploadUrlCanary**
> PresignedUploadResponseDto storageControllerRequestUploadUrlCanary(requestUploadUrlDto)

Request a presigned URL for file upload

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = StorageApi()
val requestUploadUrlDto : RequestUploadUrlDto = {"filename":"identity-document.pdf","mimeType":"application/pdf","tags":["compliance","identity-document"],"relatedEntityId":"compliance_info_123","relatedEntityType":"complianceInfo"} // RequestUploadUrlDto | 
try {
    val result : PresignedUploadResponseDto = apiInstance.storageControllerRequestUploadUrlCanary(requestUploadUrlDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StorageApi#storageControllerRequestUploadUrlCanary")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StorageApi#storageControllerRequestUploadUrlCanary")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **requestUploadUrlDto** | [**RequestUploadUrlDto**](RequestUploadUrlDto.md)|  | |

### Return type

[**PresignedUploadResponseDto**](PresignedUploadResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="storageControllerRetrieveCanary"></a>
# **storageControllerRetrieveCanary**
> FileDto storageControllerRetrieveCanary(id)

Get file details

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = StorageApi()
val id : kotlin.String = id_example // kotlin.String | File ID
try {
    val result : FileDto = apiInstance.storageControllerRetrieveCanary(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StorageApi#storageControllerRetrieveCanary")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StorageApi#storageControllerRetrieveCanary")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| File ID | |

### Return type

[**FileDto**](FileDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

