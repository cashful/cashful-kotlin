# CustomersApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createCustomer**](CustomersApi.md#createCustomer) | **POST** /api/canary/customers | Create Customer |
| [**getCustomerBalance**](CustomersApi.md#getCustomerBalance) | **GET** /api/canary/customers/{id}/balance | Get Customer&#39;s Cash Balance |
| [**listCustomerPaymentMethods**](CustomersApi.md#listCustomerPaymentMethods) | **GET** /api/canary/customers/{id}/payment-methods | List Customer&#39;s Payment Methods |
| [**listCustomerTransactions**](CustomersApi.md#listCustomerTransactions) | **GET** /api/canary/customers/{id}/transactions | List Customer&#39;s Cash Transactions |
| [**listCustomers**](CustomersApi.md#listCustomers) | **GET** /api/canary/customers | List Customers |
| [**retrieveCustomer**](CustomersApi.md#retrieveCustomer) | **GET** /api/canary/customers/{id} | Retrieve Customer |
| [**updateCustomer**](CustomersApi.md#updateCustomer) | **PATCH** /api/canary/customers/{id} | Update Customer |


<a id="createCustomer"></a>
# **createCustomer**
> CustomerResponseDto createCustomer(createCustomerDto)

Create Customer

Creates a new customer object. This also provisions their \&quot;cash balance\&quot; feature (starting at 0).

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = CustomersApi()
val createCustomerDto : CreateCustomerDto =  // CreateCustomerDto | Customer details
try {
    val result : CustomerResponseDto = apiInstance.createCustomer(createCustomerDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomersApi#createCustomer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomersApi#createCustomer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createCustomerDto** | [**CreateCustomerDto**](CreateCustomerDto.md)| Customer details | |

### Return type

[**CustomerResponseDto**](CustomerResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="getCustomerBalance"></a>
# **getCustomerBalance**
> kotlin.Any getCustomerBalance(id)

Get Customer&#39;s Cash Balance

Retrieves the real-time balance for a single customer&#39;s \&quot;cash balance\&quot; (the \&quot;wallet-enabling\&quot; feature).

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = CustomersApi()
val id : kotlin.String = id_example // kotlin.String | The unique identifier of the customer
try {
    val result : kotlin.Any = apiInstance.getCustomerBalance(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomersApi#getCustomerBalance")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomersApi#getCustomerBalance")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique identifier of the customer | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listCustomerPaymentMethods"></a>
# **listCustomerPaymentMethods**
> kotlin.Any listCustomerPaymentMethods(id)

List Customer&#39;s Payment Methods

Shows all saved payment methods (cards, etc.) for a single customer.

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = CustomersApi()
val id : kotlin.String = id_example // kotlin.String | The unique identifier of the customer
try {
    val result : kotlin.Any = apiInstance.listCustomerPaymentMethods(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomersApi#listCustomerPaymentMethods")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomersApi#listCustomerPaymentMethods")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique identifier of the customer | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listCustomerTransactions"></a>
# **listCustomerTransactions**
> ListCustomerTransactionsResponseDto listCustomerTransactions(id)

List Customer&#39;s Cash Transactions

Provides the full transaction history for a single customer&#39;s \&quot;cash balance\&quot; (Pay-Ins, Purchases, Transfers).

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = CustomersApi()
val id : kotlin.String = id_example // kotlin.String | The unique identifier of the customer
try {
    val result : ListCustomerTransactionsResponseDto = apiInstance.listCustomerTransactions(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomersApi#listCustomerTransactions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomersApi#listCustomerTransactions")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique identifier of the customer | |

### Return type

[**ListCustomerTransactionsResponseDto**](ListCustomerTransactionsResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listCustomers"></a>
# **listCustomers**
> ListCustomersResponseDto listCustomers(merchantId, search, email, limit, offset)

List Customers

Retrieves a paginated list of all customers for the merchant.

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = CustomersApi()
val merchantId : kotlin.String = merchantId_example // kotlin.String | The ID of the merchant. This parameter is required.
val search : kotlin.Any =  // kotlin.Any | Search across customer fields
val email : kotlin.Any =  // kotlin.Any | Filter by email address
val limit : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Maximum number of records to return
val offset : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Number of records to skip
try {
    val result : ListCustomersResponseDto = apiInstance.listCustomers(merchantId, search, email, limit, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomersApi#listCustomers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomersApi#listCustomers")
    e.printStackTrace()
}
```

### Parameters
| **merchantId** | **kotlin.String**| The ID of the merchant. This parameter is required. | |
| **search** | [**kotlin.Any**](.md)| Search across customer fields | [optional] |
| **email** | [**kotlin.Any**](.md)| Filter by email address | [optional] |
| **limit** | **java.math.BigDecimal**| Maximum number of records to return | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **offset** | **java.math.BigDecimal**| Number of records to skip | [optional] |

### Return type

[**ListCustomersResponseDto**](ListCustomersResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="retrieveCustomer"></a>
# **retrieveCustomer**
> kotlin.Any retrieveCustomer(id)

Retrieve Customer

Gets the details for a single customer.

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = CustomersApi()
val id : kotlin.String = id_example // kotlin.String | The unique identifier of the customer
try {
    val result : kotlin.Any = apiInstance.retrieveCustomer(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomersApi#retrieveCustomer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomersApi#retrieveCustomer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The unique identifier of the customer | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="updateCustomer"></a>
# **updateCustomer**
> kotlin.Any updateCustomer(id, updateCustomerDto)

Update Customer

Updates a customer&#39;s details (e.g., email, metadata).

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = CustomersApi()
val id : kotlin.String = id_example // kotlin.String | The unique identifier of the customer
val updateCustomerDto : UpdateCustomerDto =  // UpdateCustomerDto | Customer update details
try {
    val result : kotlin.Any = apiInstance.updateCustomer(id, updateCustomerDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomersApi#updateCustomer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomersApi#updateCustomer")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The unique identifier of the customer | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateCustomerDto** | [**UpdateCustomerDto**](UpdateCustomerDto.md)| Customer update details | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

