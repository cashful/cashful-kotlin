# TransfersApi

All URIs are relative to *http://localhost:9000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createTransfer**](TransfersApi.md#createTransfer) | **POST** /api/canary/transfers | Create P2P Transfer |


<a id="createTransfer"></a>
# **createTransfer**
> TransferResponseDto createTransfer(createTransferDto)

Create P2P Transfer

(Wallet-Enabling) Moves funds from one CustomerBalance to another CustomerBalance. This is the P2P feature.

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = TransfersApi()
val createTransferDto : CreateTransferDto =  // CreateTransferDto | Transfer details
try {
    val result : TransferResponseDto = apiInstance.createTransfer(createTransferDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TransfersApi#createTransfer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TransfersApi#createTransfer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createTransferDto** | [**CreateTransferDto**](CreateTransferDto.md)| Transfer details | |

### Return type

[**TransferResponseDto**](TransferResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

