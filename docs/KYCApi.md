# KYCApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createKyc**](KYCApi.md#createKyc) | **POST** /api/canary/kyc | Create KYC info |
| [**getKyc**](KYCApi.md#getKyc) | **GET** /api/canary/kyc | Get KYC info for organization |
| [**updateKyc**](KYCApi.md#updateKyc) | **PATCH** /api/canary/kyc/{id} | Update KYC info |


<a id="createKyc"></a>
# **createKyc**
> OrganizationKycResponseDto createKyc(createOrganizationKycDto)

Create KYC info

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = KYCApi()
val createOrganizationKycDto : CreateOrganizationKycDto =  // CreateOrganizationKycDto | 
try {
    val result : OrganizationKycResponseDto = apiInstance.createKyc(createOrganizationKycDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KYCApi#createKyc")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KYCApi#createKyc")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createOrganizationKycDto** | [**CreateOrganizationKycDto**](CreateOrganizationKycDto.md)|  | |

### Return type

[**OrganizationKycResponseDto**](OrganizationKycResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="getKyc"></a>
# **getKyc**
> OrganizationKycResponseDto getKyc(organizationId)

Get KYC info for organization

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = KYCApi()
val organizationId : kotlin.String = organizationId_example // kotlin.String | 
try {
    val result : OrganizationKycResponseDto = apiInstance.getKyc(organizationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KYCApi#getKyc")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KYCApi#getKyc")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **organizationId** | **kotlin.String**|  | |

### Return type

[**OrganizationKycResponseDto**](OrganizationKycResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="updateKyc"></a>
# **updateKyc**
> updateKyc(id, updateOrganizationKycDto)

Update KYC info

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = KYCApi()
val id : kotlin.String = id_example // kotlin.String | 
val updateOrganizationKycDto : UpdateOrganizationKycDto =  // UpdateOrganizationKycDto | 
try {
    apiInstance.updateKyc(id, updateOrganizationKycDto)
} catch (e: ClientException) {
    println("4xx response calling KYCApi#updateKyc")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KYCApi#updateKyc")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateOrganizationKycDto** | [**UpdateOrganizationKycDto**](UpdateOrganizationKycDto.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

