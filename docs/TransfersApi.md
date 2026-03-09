# TransfersApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createTransfer**](TransfersApi.md#createTransfer) | **POST** /api/canary/transfers | Create P2P Transfer |
| [**listTransfers**](TransfersApi.md#listTransfers) | **GET** /api/canary/transfers | List Transfers |


<a id="createTransfer"></a>
# **createTransfer**
> TransferResponseDto createTransfer(createTransferDto)

Create P2P Transfer

(Wallet-Enabling) Moves funds from one CustomerBalance to another CustomerBalance. This is the P2P feature.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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

<a id="listTransfers"></a>
# **listTransfers**
> ListTransfersResponseDto listTransfers(limit, offset, filter, sort, order, merchantId)

List Transfers

Lists transfers for a specific merchant with pagination.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = TransfersApi()
val limit : java.math.BigDecimal = 50 // java.math.BigDecimal | Maximum number of items to return
val offset : java.math.BigDecimal = 0 // java.math.BigDecimal | Number of items to skip
val filter : kotlin.String = {"ids":["prod_123","prod_456"]} // kotlin.String | JSON string used for dynamic filtering
val sort : kotlin.String = createdAt // kotlin.String | Field name to sort by
val order : kotlin.String = DESC // kotlin.String | Sort direction
val merchantId : kotlin.String = merchantId_example // kotlin.String | Filter by merchant ID. If omitted, defaults to the authenticated merchant.
try {
    val result : ListTransfersResponseDto = apiInstance.listTransfers(limit, offset, filter, sort, order, merchantId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TransfersApi#listTransfers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TransfersApi#listTransfers")
    e.printStackTrace()
}
```

### Parameters
| **limit** | **java.math.BigDecimal**| Maximum number of items to return | [optional] |
| **offset** | **java.math.BigDecimal**| Number of items to skip | [optional] |
| **filter** | **kotlin.String**| JSON string used for dynamic filtering | [optional] |
| **sort** | **kotlin.String**| Field name to sort by | [optional] |
| **order** | **kotlin.String**| Sort direction | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **merchantId** | **kotlin.String**| Filter by merchant ID. If omitted, defaults to the authenticated merchant. | [optional] |

### Return type

[**ListTransfersResponseDto**](ListTransfersResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

