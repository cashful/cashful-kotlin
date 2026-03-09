# ComplianceApi

All URIs are relative to *https://api.cashful.africa*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createCompliance**](ComplianceApi.md#createCompliance) | **POST** /api/canary/compliance | Create Compliance info |
| [**listCompliance**](ComplianceApi.md#listCompliance) | **GET** /api/canary/compliance | List Compliance info for organization |
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

<a id="listCompliance"></a>
# **listCompliance**
> ListOrganizationComplianceResponseDto listCompliance(limit, offset, filter, sort, order)

List Compliance info for organization

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = ComplianceApi()
val limit : java.math.BigDecimal = 50 // java.math.BigDecimal | Maximum number of items to return
val offset : java.math.BigDecimal = 0 // java.math.BigDecimal | Number of items to skip
val filter : kotlin.String = {"ids":["prod_123","prod_456"]} // kotlin.String | JSON string used for dynamic filtering
val sort : kotlin.String = createdAt // kotlin.String | Field name to sort by
val order : kotlin.String = DESC // kotlin.String | Sort direction
try {
    val result : ListOrganizationComplianceResponseDto = apiInstance.listCompliance(limit, offset, filter, sort, order)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComplianceApi#listCompliance")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComplianceApi#listCompliance")
    e.printStackTrace()
}
```

### Parameters
| **limit** | **java.math.BigDecimal**| Maximum number of items to return | [optional] |
| **offset** | **java.math.BigDecimal**| Number of items to skip | [optional] |
| **filter** | **kotlin.String**| JSON string used for dynamic filtering | [optional] |
| **sort** | **kotlin.String**| Field name to sort by | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **order** | **kotlin.String**| Sort direction | [optional] |

### Return type

[**ListOrganizationComplianceResponseDto**](ListOrganizationComplianceResponseDto.md)

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

