# StorageApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**confirmUpload**](StorageApi.md#confirmUpload) | **POST** /api/canary/storage/confirm-upload | Confirm that a file upload was completed |
| [**deleteFile**](StorageApi.md#deleteFile) | **DELETE** /api/canary/storage/{id} | Delete a file |
| [**getDownloadUrl**](StorageApi.md#getDownloadUrl) | **GET** /api/canary/storage/{id}/download-url | Get a presigned download URL for a file |
| [**getFileDetails**](StorageApi.md#getFileDetails) | **GET** /api/canary/storage/{id} | Get file details |
| [**listFiles**](StorageApi.md#listFiles) | **GET** /api/canary/storage | List files |
| [**requestUploadUrl**](StorageApi.md#requestUploadUrl) | **POST** /api/canary/storage/upload-url | Request a presigned URL for file upload |


<a id="confirmUpload"></a>
# **confirmUpload**
> FileDto confirmUpload(confirmUploadDto)

Confirm that a file upload was completed

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = StorageApi()
val confirmUploadDto : ConfirmUploadDto = {"fileId":"file_abc123xyz","checksum":"sha256:a1b2c3d4e5f6...","size":245760} // ConfirmUploadDto | 
try {
    val result : FileDto = apiInstance.confirmUpload(confirmUploadDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StorageApi#confirmUpload")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StorageApi#confirmUpload")
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

<a id="deleteFile"></a>
# **deleteFile**
> deleteFile(id)

Delete a file

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = StorageApi()
val id : kotlin.String = id_example // kotlin.String | File ID
try {
    apiInstance.deleteFile(id)
} catch (e: ClientException) {
    println("4xx response calling StorageApi#deleteFile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StorageApi#deleteFile")
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

<a id="getDownloadUrl"></a>
# **getDownloadUrl**
> PresignedDownloadResponseDto getDownloadUrl(id)

Get a presigned download URL for a file

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = StorageApi()
val id : kotlin.String = id_example // kotlin.String | File ID
try {
    val result : PresignedDownloadResponseDto = apiInstance.getDownloadUrl(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StorageApi#getDownloadUrl")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StorageApi#getDownloadUrl")
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

<a id="getFileDetails"></a>
# **getFileDetails**
> FileDto getFileDetails(id)

Get file details

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = StorageApi()
val id : kotlin.String = id_example // kotlin.String | File ID
try {
    val result : FileDto = apiInstance.getFileDetails(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StorageApi#getFileDetails")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StorageApi#getFileDetails")
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

<a id="listFiles"></a>
# **listFiles**
> ListFilesResponseDto listFiles(limit, offset, tag, status, relatedEntityId, relatedEntityType)

List files

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = StorageApi()
val limit : java.math.BigDecimal = 50 // java.math.BigDecimal | Maximum number of records to return
val offset : java.math.BigDecimal = 0 // java.math.BigDecimal | Number of records to skip
val tag : kotlin.String = tag_example // kotlin.String | Filter by tag
val status : kotlin.String = status_example // kotlin.String | 
val relatedEntityId : kotlin.String = relatedEntityId_example // kotlin.String | 
val relatedEntityType : kotlin.String = relatedEntityType_example // kotlin.String | 
try {
    val result : ListFilesResponseDto = apiInstance.listFiles(limit, offset, tag, status, relatedEntityId, relatedEntityType)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StorageApi#listFiles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StorageApi#listFiles")
    e.printStackTrace()
}
```

### Parameters
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

<a id="requestUploadUrl"></a>
# **requestUploadUrl**
> PresignedUploadResponseDto requestUploadUrl(requestUploadUrlDto)

Request a presigned URL for file upload

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = StorageApi()
val requestUploadUrlDto : RequestUploadUrlDto = {"filename":"iphone-15.png","mimeType":"image/png","isPublic":true,"tags":["product","image"],"relatedEntityId":"product_123","relatedEntityType":"product"} // RequestUploadUrlDto | 
try {
    val result : PresignedUploadResponseDto = apiInstance.requestUploadUrl(requestUploadUrlDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StorageApi#requestUploadUrl")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StorageApi#requestUploadUrl")
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

