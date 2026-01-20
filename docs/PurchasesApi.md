# PurchasesApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createPurchase**](PurchasesApi.md#createPurchase) | **POST** /api/canary/purchases | Buy with Cash Balance |


<a id="createPurchase"></a>
# **createPurchase**
> PurchaseResponseDto createPurchase(createPurchaseDto)

Buy with Cash Balance

(Wallet-Enabling) Spends a product using the CustomerBalance as the source. Atomically debits the CustomerBalance and credits the MerchantBalance.

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = PurchasesApi()
val createPurchaseDto : CreatePurchaseDto =  // CreatePurchaseDto | Purchase details
try {
    val result : PurchaseResponseDto = apiInstance.createPurchase(createPurchaseDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PurchasesApi#createPurchase")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PurchasesApi#createPurchase")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createPurchaseDto** | [**CreatePurchaseDto**](CreatePurchaseDto.md)| Purchase details | |

### Return type

[**PurchaseResponseDto**](PurchaseResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

