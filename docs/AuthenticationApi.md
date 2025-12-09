# AuthenticationApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**acceptInvitation**](AuthenticationApi.md#acceptInvitation) | **POST** /api/canary/authentication/organization/accept-invitation | Accept Invitation |
| [**cancelInvitation**](AuthenticationApi.md#cancelInvitation) | **POST** /api/canary/authentication/organization/cancel-invitation | Cancel Invitation |
| [**createApiKey**](AuthenticationApi.md#createApiKey) | **POST** /api/canary/authentication/api-key/create | Create API Key |
| [**createOrganization**](AuthenticationApi.md#createOrganization) | **POST** /api/canary/authentication/organization/create | Create Organization |
| [**deleteApiKey**](AuthenticationApi.md#deleteApiKey) | **POST** /api/canary/authentication/api-key/delete | Delete API Key |
| [**deleteOrganization**](AuthenticationApi.md#deleteOrganization) | **POST** /api/canary/authentication/organization/delete | Delete Organization |
| [**forgetPassword**](AuthenticationApi.md#forgetPassword) | **POST** /api/canary/authentication/forget-password | Forget Password |
| [**getSession**](AuthenticationApi.md#getSession) | **GET** /api/canary/authentication/get-session | Get Session |
| [**inviteMember**](AuthenticationApi.md#inviteMember) | **POST** /api/canary/authentication/organization/invite-member | Invite Member |
| [**listApiKeys**](AuthenticationApi.md#listApiKeys) | **GET** /api/canary/authentication/api-key/list | List API Keys |
| [**listOrganizations**](AuthenticationApi.md#listOrganizations) | **GET** /api/canary/authentication/organization/list | List Organizations |
| [**rejectInvitation**](AuthenticationApi.md#rejectInvitation) | **POST** /api/canary/authentication/organization/reject-invitation | Reject Invitation |
| [**removeMember**](AuthenticationApi.md#removeMember) | **POST** /api/canary/authentication/organization/remove-member | Remove Member |
| [**resetPassword**](AuthenticationApi.md#resetPassword) | **POST** /api/canary/authentication/reset-password | Reset Password |
| [**setActiveOrganization**](AuthenticationApi.md#setActiveOrganization) | **POST** /api/canary/authentication/organization/set-active | Set Active Organization |
| [**signInEmail**](AuthenticationApi.md#signInEmail) | **POST** /api/canary/authentication/sign-in/email | Sign in with email |
| [**signOut**](AuthenticationApi.md#signOut) | **POST** /api/canary/authentication/sign-out | Sign out |
| [**signUpEmail**](AuthenticationApi.md#signUpEmail) | **POST** /api/canary/authentication/sign-up/email | Sign up with email |
| [**updateApiKey**](AuthenticationApi.md#updateApiKey) | **POST** /api/canary/authentication/api-key/update | Update API Key |
| [**updateMemberRole**](AuthenticationApi.md#updateMemberRole) | **POST** /api/canary/authentication/organization/update-member-role | Update Member Role |
| [**updateOrganization**](AuthenticationApi.md#updateOrganization) | **POST** /api/canary/authentication/organization/update | Update Organization |
| [**verifyApiKey**](AuthenticationApi.md#verifyApiKey) | **POST** /api/canary/authentication/api-key/verify | Verify API Key |


<a id="acceptInvitation"></a>
# **acceptInvitation**
> acceptInvitation(acceptInvitationDto)

Accept Invitation

Accept an invitation to an organization

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val acceptInvitationDto : AcceptInvitationDto =  // AcceptInvitationDto | 
try {
    apiInstance.acceptInvitation(acceptInvitationDto)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#acceptInvitation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#acceptInvitation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **acceptInvitationDto** | [**AcceptInvitationDto**](AcceptInvitationDto.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="cancelInvitation"></a>
# **cancelInvitation**
> cancelInvitation(cancelInvitationDto)

Cancel Invitation

Cancel an invitation to an organization

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val cancelInvitationDto : CancelInvitationDto =  // CancelInvitationDto | 
try {
    apiInstance.cancelInvitation(cancelInvitationDto)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#cancelInvitation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#cancelInvitation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cancelInvitationDto** | [**CancelInvitationDto**](CancelInvitationDto.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="createApiKey"></a>
# **createApiKey**
> createApiKey(createApiKeyDto)

Create API Key

Create a new API key

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val createApiKeyDto : CreateApiKeyDto =  // CreateApiKeyDto | 
try {
    apiInstance.createApiKey(createApiKeyDto)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#createApiKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#createApiKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createApiKeyDto** | [**CreateApiKeyDto**](CreateApiKeyDto.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="createOrganization"></a>
# **createOrganization**
> createOrganization(createOrganizationDto)

Create Organization

Create a new organization

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val createOrganizationDto : CreateOrganizationDto =  // CreateOrganizationDto | 
try {
    apiInstance.createOrganization(createOrganizationDto)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#createOrganization")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#createOrganization")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createOrganizationDto** | [**CreateOrganizationDto**](CreateOrganizationDto.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="deleteApiKey"></a>
# **deleteApiKey**
> deleteApiKey(deleteApiKeyDto)

Delete API Key

Delete an API key

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val deleteApiKeyDto : DeleteApiKeyDto =  // DeleteApiKeyDto | 
try {
    apiInstance.deleteApiKey(deleteApiKeyDto)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#deleteApiKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#deleteApiKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **deleteApiKeyDto** | [**DeleteApiKeyDto**](DeleteApiKeyDto.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="deleteOrganization"></a>
# **deleteOrganization**
> deleteOrganization(deleteOrganizationDto)

Delete Organization

Delete an organization

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val deleteOrganizationDto : DeleteOrganizationDto =  // DeleteOrganizationDto | 
try {
    apiInstance.deleteOrganization(deleteOrganizationDto)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#deleteOrganization")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#deleteOrganization")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **deleteOrganizationDto** | [**DeleteOrganizationDto**](DeleteOrganizationDto.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="forgetPassword"></a>
# **forgetPassword**
> forgetPassword(forgotPasswordDto)

Forget Password

Send a password reset email to the user

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val forgotPasswordDto : ForgotPasswordDto =  // ForgotPasswordDto | 
try {
    apiInstance.forgetPassword(forgotPasswordDto)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#forgetPassword")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#forgetPassword")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **forgotPasswordDto** | [**ForgotPasswordDto**](ForgotPasswordDto.md)|  | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="getSession"></a>
# **getSession**
> GetSessionResponseDto getSession()

Get Session

Retrieve the current user session

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
try {
    val result : GetSessionResponseDto = apiInstance.getSession()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#getSession")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#getSession")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**GetSessionResponseDto**](GetSessionResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="inviteMember"></a>
# **inviteMember**
> inviteMember(inviteMemberDto)

Invite Member

Invite a user to an organization

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val inviteMemberDto : InviteMemberDto =  // InviteMemberDto | 
try {
    apiInstance.inviteMember(inviteMemberDto)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#inviteMember")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#inviteMember")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **inviteMemberDto** | [**InviteMemberDto**](InviteMemberDto.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="listApiKeys"></a>
# **listApiKeys**
> listApiKeys()

List API Keys

List all API keys for the current user

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
try {
    apiInstance.listApiKeys()
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#listApiKeys")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#listApiKeys")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listOrganizations"></a>
# **listOrganizations**
> listOrganizations()

List Organizations

List all organizations for the current user

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
try {
    apiInstance.listOrganizations()
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#listOrganizations")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#listOrganizations")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="rejectInvitation"></a>
# **rejectInvitation**
> rejectInvitation(rejectInvitationDto)

Reject Invitation

Reject an invitation to an organization

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val rejectInvitationDto : RejectInvitationDto =  // RejectInvitationDto | 
try {
    apiInstance.rejectInvitation(rejectInvitationDto)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#rejectInvitation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#rejectInvitation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **rejectInvitationDto** | [**RejectInvitationDto**](RejectInvitationDto.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="removeMember"></a>
# **removeMember**
> removeMember(removeMemberDto)

Remove Member

Remove a member from an organization

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val removeMemberDto : RemoveMemberDto =  // RemoveMemberDto | 
try {
    apiInstance.removeMember(removeMemberDto)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#removeMember")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#removeMember")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **removeMemberDto** | [**RemoveMemberDto**](RemoveMemberDto.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="resetPassword"></a>
# **resetPassword**
> resetPassword(resetPasswordDto)

Reset Password

Reset the user&#39;s password using a token

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val resetPasswordDto : ResetPasswordDto =  // ResetPasswordDto | 
try {
    apiInstance.resetPassword(resetPasswordDto)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#resetPassword")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#resetPassword")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **resetPasswordDto** | [**ResetPasswordDto**](ResetPasswordDto.md)|  | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="setActiveOrganization"></a>
# **setActiveOrganization**
> setActiveOrganization(setActiveOrganizationDto)

Set Active Organization

Set the active organization for the current session

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val setActiveOrganizationDto : SetActiveOrganizationDto =  // SetActiveOrganizationDto | 
try {
    apiInstance.setActiveOrganization(setActiveOrganizationDto)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#setActiveOrganization")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#setActiveOrganization")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **setActiveOrganizationDto** | [**SetActiveOrganizationDto**](SetActiveOrganizationDto.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="signInEmail"></a>
# **signInEmail**
> signInEmail(signInDto)

Sign in with email

Authenticate a user using email and password

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val signInDto : SignInDto =  // SignInDto | 
try {
    apiInstance.signInEmail(signInDto)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#signInEmail")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#signInEmail")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **signInDto** | [**SignInDto**](SignInDto.md)|  | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="signOut"></a>
# **signOut**
> signOut()

Sign out

Sign out the current user and invalidate the session

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
try {
    apiInstance.signOut()
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#signOut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#signOut")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="signUpEmail"></a>
# **signUpEmail**
> signUpEmail(signUpDto)

Sign up with email

Create a new user account using email and password

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val signUpDto : SignUpDto =  // SignUpDto | 
try {
    apiInstance.signUpEmail(signUpDto)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#signUpEmail")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#signUpEmail")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **signUpDto** | [**SignUpDto**](SignUpDto.md)|  | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="updateApiKey"></a>
# **updateApiKey**
> updateApiKey(updateApiKeyDto)

Update API Key

Update an API key

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val updateApiKeyDto : UpdateApiKeyDto =  // UpdateApiKeyDto | 
try {
    apiInstance.updateApiKey(updateApiKeyDto)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#updateApiKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#updateApiKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateApiKeyDto** | [**UpdateApiKeyDto**](UpdateApiKeyDto.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="updateMemberRole"></a>
# **updateMemberRole**
> updateMemberRole(updateMemberRoleDto)

Update Member Role

Update a member&#39;s role in an organization

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val updateMemberRoleDto : UpdateMemberRoleDto =  // UpdateMemberRoleDto | 
try {
    apiInstance.updateMemberRole(updateMemberRoleDto)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#updateMemberRole")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#updateMemberRole")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateMemberRoleDto** | [**UpdateMemberRoleDto**](UpdateMemberRoleDto.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="updateOrganization"></a>
# **updateOrganization**
> updateOrganization(updateOrganizationDto)

Update Organization

Update an organization&#39;s details

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val updateOrganizationDto : UpdateOrganizationDto =  // UpdateOrganizationDto | 
try {
    apiInstance.updateOrganization(updateOrganizationDto)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#updateOrganization")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#updateOrganization")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateOrganizationDto** | [**UpdateOrganizationDto**](UpdateOrganizationDto.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="verifyApiKey"></a>
# **verifyApiKey**
> verifyApiKey(verifyApiKeyDto)

Verify API Key

Verify an API key

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val verifyApiKeyDto : VerifyApiKeyDto =  // VerifyApiKeyDto | 
try {
    apiInstance.verifyApiKey(verifyApiKeyDto)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#verifyApiKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#verifyApiKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **verifyApiKeyDto** | [**VerifyApiKeyDto**](VerifyApiKeyDto.md)|  | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

