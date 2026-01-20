# ComplianceApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createCompliance**](ComplianceApi.md#createCompliance) | **POST** /api/canary/compliance | Create Compliance info |
| [**getCompliance**](ComplianceApi.md#getCompliance) | **GET** /api/canary/compliance | Get Compliance info for organization |
| [**updateCompliance**](ComplianceApi.md#updateCompliance) | **PATCH** /api/canary/compliance/{id} | Update Compliance info |


<a id="createCompliance"></a>
# **createCompliance**
> OrganizationComplianceResponseDto createCompliance(createOrganizationComplianceDto)

Create Compliance info

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = ComplianceApi()
val createOrganizationComplianceDto : CreateOrganizationComplianceDto =  // CreateOrganizationComplianceDto | 
try {
    val result : OrganizationComplianceResponseDto = apiInstance.createCompliance(createOrganizationComplianceDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComplianceApi#createCompliance")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComplianceApi#createCompliance")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createOrganizationComplianceDto** | [**CreateOrganizationComplianceDto**](CreateOrganizationComplianceDto.md)|  | |

### Return type

[**OrganizationComplianceResponseDto**](OrganizationComplianceResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="getCompliance"></a>
# **getCompliance**
> OrganizationComplianceResponseDto getCompliance(organizationId)

Get Compliance info for organization

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = ComplianceApi()
val organizationId : kotlin.String = organizationId_example // kotlin.String | 
try {
    val result : OrganizationComplianceResponseDto = apiInstance.getCompliance(organizationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComplianceApi#getCompliance")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComplianceApi#getCompliance")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **organizationId** | **kotlin.String**|  | |

### Return type

[**OrganizationComplianceResponseDto**](OrganizationComplianceResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="updateCompliance"></a>
# **updateCompliance**
> updateCompliance(id, updateOrganizationComplianceDto)

Update Compliance info

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = ComplianceApi()
val id : kotlin.String = id_example // kotlin.String | 
val updateOrganizationComplianceDto : UpdateOrganizationComplianceDto =  // UpdateOrganizationComplianceDto | 
try {
    apiInstance.updateCompliance(id, updateOrganizationComplianceDto)
} catch (e: ClientException) {
    println("4xx response calling ComplianceApi#updateCompliance")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComplianceApi#updateCompliance")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateOrganizationComplianceDto** | [**UpdateOrganizationComplianceDto**](UpdateOrganizationComplianceDto.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

