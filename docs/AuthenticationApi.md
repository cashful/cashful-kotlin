# AuthenticationApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**acceptInvitation**](AuthenticationApi.md#acceptInvitation) | **POST** /api/canary/authentication/organization/accept-invitation | Accept Invitation |
| [**cancelInvitation**](AuthenticationApi.md#cancelInvitation) | **POST** /api/canary/authentication/organization/cancel-invitation | Cancel Invitation |
| [**changeEmail**](AuthenticationApi.md#changeEmail) | **POST** /api/canary/authentication/change-email | Change Email |
| [**changePassword**](AuthenticationApi.md#changePassword) | **POST** /api/canary/authentication/change-password | Change Password |
| [**checkSlug**](AuthenticationApi.md#checkSlug) | **POST** /api/canary/authentication/organization/check-slug | Check Slug |
| [**createApiKey**](AuthenticationApi.md#createApiKey) | **POST** /api/canary/authentication/api-key/create | Create API Key |
| [**createOrganization**](AuthenticationApi.md#createOrganization) | **POST** /api/canary/authentication/organization/create | Create Organization |
| [**deleteApiKey**](AuthenticationApi.md#deleteApiKey) | **POST** /api/canary/authentication/api-key/delete | Delete API Key |
| [**deleteOrganization**](AuthenticationApi.md#deleteOrganization) | **POST** /api/canary/authentication/organization/delete | Delete Organization |
| [**deleteUser**](AuthenticationApi.md#deleteUser) | **POST** /api/canary/authentication/delete-user | Delete User |
| [**forgetPassword**](AuthenticationApi.md#forgetPassword) | **POST** /api/canary/authentication/forget-password | Forget Password |
| [**getActiveMember**](AuthenticationApi.md#getActiveMember) | **GET** /api/canary/authentication/organization/get-active-member | Get Active Member |
| [**getActiveMemberRole**](AuthenticationApi.md#getActiveMemberRole) | **GET** /api/canary/authentication/organization/get-active-member-role | Get Active Member Role |
| [**getInvitation**](AuthenticationApi.md#getInvitation) | **GET** /api/canary/authentication/organization/get-invitation | Get Invitation |
| [**getOrganization**](AuthenticationApi.md#getOrganization) | **GET** /api/canary/authentication/organization/get-full-organization | Get Full Organization |
| [**getSession**](AuthenticationApi.md#getSession) | **GET** /api/canary/authentication/get-session | Get Session |
| [**hasPermission**](AuthenticationApi.md#hasPermission) | **POST** /api/canary/authentication/organization/has-permission | Has Permission |
| [**inviteMember**](AuthenticationApi.md#inviteMember) | **POST** /api/canary/authentication/organization/invite-member | Invite Member |
| [**leaveOrganization**](AuthenticationApi.md#leaveOrganization) | **POST** /api/canary/authentication/organization/leave | Leave Organization |
| [**listApiKeys**](AuthenticationApi.md#listApiKeys) | **GET** /api/canary/authentication/api-key/list | List API Keys |
| [**listMembers**](AuthenticationApi.md#listMembers) | **GET** /api/canary/authentication/organization/list-members | List Members |
| [**listOrganizationInvitations**](AuthenticationApi.md#listOrganizationInvitations) | **GET** /api/canary/authentication/organization/list-invitations | List Invitations |
| [**listOrganizations**](AuthenticationApi.md#listOrganizations) | **GET** /api/canary/authentication/organization/list | List Organizations |
| [**listUserInvitations**](AuthenticationApi.md#listUserInvitations) | **GET** /api/canary/authentication/organization/list-user-invitations | List User Invitations |
| [**listUserSessions**](AuthenticationApi.md#listUserSessions) | **GET** /api/canary/authentication/list-sessions | List User Sessions |
| [**rejectInvitation**](AuthenticationApi.md#rejectInvitation) | **POST** /api/canary/authentication/organization/reject-invitation | Reject Invitation |
| [**removeMember**](AuthenticationApi.md#removeMember) | **POST** /api/canary/authentication/organization/remove-member | Remove Member |
| [**requestPasswordReset**](AuthenticationApi.md#requestPasswordReset) | **POST** /api/canary/authentication/request-password-reset | Request Password Reset |
| [**resetPassword**](AuthenticationApi.md#resetPassword) | **POST** /api/canary/authentication/reset-password | Reset Password |
| [**resetPasswordCallback**](AuthenticationApi.md#resetPasswordCallback) | **GET** /api/canary/authentication/reset-password/{token} | Reset Password Callback |
| [**revokeSession**](AuthenticationApi.md#revokeSession) | **POST** /api/canary/authentication/revoke-session | Revoke Session |
| [**sendVerificationEmail**](AuthenticationApi.md#sendVerificationEmail) | **POST** /api/canary/authentication/send-verification-email | Send Verification Email |
| [**setActiveOrganization**](AuthenticationApi.md#setActiveOrganization) | **POST** /api/canary/authentication/organization/set-active | Set Active Organization |
| [**signInEmail**](AuthenticationApi.md#signInEmail) | **POST** /api/canary/authentication/sign-in/email | Sign in with email |
| [**signOut**](AuthenticationApi.md#signOut) | **POST** /api/canary/authentication/sign-out | Sign out |
| [**signUpEmail**](AuthenticationApi.md#signUpEmail) | **POST** /api/canary/authentication/sign-up/email | Sign up with email |
| [**updateApiKey**](AuthenticationApi.md#updateApiKey) | **POST** /api/canary/authentication/api-key/update | Update API Key |
| [**updateMemberRole**](AuthenticationApi.md#updateMemberRole) | **POST** /api/canary/authentication/organization/update-member-role | Update Member Role |
| [**updateOrganization**](AuthenticationApi.md#updateOrganization) | **POST** /api/canary/authentication/organization/update | Update Organization |
| [**updateUser**](AuthenticationApi.md#updateUser) | **POST** /api/canary/authentication/update-user | Update User |
| [**verifyApiKey**](AuthenticationApi.md#verifyApiKey) | **POST** /api/canary/authentication/api-key/verify | Verify API Key |
| [**verifyEmail**](AuthenticationApi.md#verifyEmail) | **GET** /api/canary/authentication/verify-email | Verify Email |


<a id="acceptInvitation"></a>
# **acceptInvitation**
> AcceptInvitationResponseDto acceptInvitation(acceptInvitationDto)

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
    val result : AcceptInvitationResponseDto = apiInstance.acceptInvitation(acceptInvitationDto)
    println(result)
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

[**AcceptInvitationResponseDto**](AcceptInvitationResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="cancelInvitation"></a>
# **cancelInvitation**
> CancelInvitationResponseDto cancelInvitation(cancelInvitationDto)

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
    val result : CancelInvitationResponseDto = apiInstance.cancelInvitation(cancelInvitationDto)
    println(result)
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

[**CancelInvitationResponseDto**](CancelInvitationResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="changeEmail"></a>
# **changeEmail**
> ChangeEmailResponseDto changeEmail(changeEmailDto)

Change Email

Change the email address of the current user

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val changeEmailDto : ChangeEmailDto =  // ChangeEmailDto | 
try {
    val result : ChangeEmailResponseDto = apiInstance.changeEmail(changeEmailDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#changeEmail")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#changeEmail")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **changeEmailDto** | [**ChangeEmailDto**](ChangeEmailDto.md)|  | |

### Return type

[**ChangeEmailResponseDto**](ChangeEmailResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="changePassword"></a>
# **changePassword**
> ChangePasswordResponseDto changePassword(changePasswordDto)

Change Password

Change the password of the current user

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val changePasswordDto : ChangePasswordDto =  // ChangePasswordDto | 
try {
    val result : ChangePasswordResponseDto = apiInstance.changePassword(changePasswordDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#changePassword")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#changePassword")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **changePasswordDto** | [**ChangePasswordDto**](ChangePasswordDto.md)|  | |

### Return type

[**ChangePasswordResponseDto**](ChangePasswordResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="checkSlug"></a>
# **checkSlug**
> CheckSlugResponseDto checkSlug(checkSlugDto)

Check Slug

Check if organization slug is available

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val checkSlugDto : CheckSlugDto =  // CheckSlugDto | 
try {
    val result : CheckSlugResponseDto = apiInstance.checkSlug(checkSlugDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#checkSlug")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#checkSlug")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **checkSlugDto** | [**CheckSlugDto**](CheckSlugDto.md)|  | |

### Return type

[**CheckSlugResponseDto**](CheckSlugResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="createApiKey"></a>
# **createApiKey**
> CreateApiKeyResponseDto createApiKey(createApiKeyDto)

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
    val result : CreateApiKeyResponseDto = apiInstance.createApiKey(createApiKeyDto)
    println(result)
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

[**CreateApiKeyResponseDto**](CreateApiKeyResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="createOrganization"></a>
# **createOrganization**
> CreateOrganizationResponseDto createOrganization(createOrganizationDto)

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
    val result : CreateOrganizationResponseDto = apiInstance.createOrganization(createOrganizationDto)
    println(result)
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

[**CreateOrganizationResponseDto**](CreateOrganizationResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="deleteApiKey"></a>
# **deleteApiKey**
> DeleteApiKeyResponseDto deleteApiKey(deleteApiKeyDto)

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
    val result : DeleteApiKeyResponseDto = apiInstance.deleteApiKey(deleteApiKeyDto)
    println(result)
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

[**DeleteApiKeyResponseDto**](DeleteApiKeyResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="deleteOrganization"></a>
# **deleteOrganization**
> DeleteOrganizationResponseDto deleteOrganization(deleteOrganizationDto)

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
    val result : DeleteOrganizationResponseDto = apiInstance.deleteOrganization(deleteOrganizationDto)
    println(result)
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

[**DeleteOrganizationResponseDto**](DeleteOrganizationResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="deleteUser"></a>
# **deleteUser**
> DeleteUserResponseDto deleteUser(deleteUserDto)

Delete User

Delete the current user&#39;s account

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val deleteUserDto : DeleteUserDto =  // DeleteUserDto | 
try {
    val result : DeleteUserResponseDto = apiInstance.deleteUser(deleteUserDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#deleteUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#deleteUser")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **deleteUserDto** | [**DeleteUserDto**](DeleteUserDto.md)|  | |

### Return type

[**DeleteUserResponseDto**](DeleteUserResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="forgetPassword"></a>
# **forgetPassword**
> ForgotPasswordResponseDto forgetPassword(forgotPasswordDto)

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
    val result : ForgotPasswordResponseDto = apiInstance.forgetPassword(forgotPasswordDto)
    println(result)
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

[**ForgotPasswordResponseDto**](ForgotPasswordResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="getActiveMember"></a>
# **getActiveMember**
> GetActiveMemberResponseDto getActiveMember(organizationId)

Get Active Member

Get the member details of the active organization

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val organizationId : kotlin.String = org_12345 // kotlin.String | Filter by organization ID
try {
    val result : GetActiveMemberResponseDto = apiInstance.getActiveMember(organizationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#getActiveMember")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#getActiveMember")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **organizationId** | **kotlin.String**| Filter by organization ID | [optional] |

### Return type

[**GetActiveMemberResponseDto**](GetActiveMemberResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getActiveMemberRole"></a>
# **getActiveMemberRole**
> GetActiveMemberRoleResponseDto getActiveMemberRole(organizationId)

Get Active Member Role

Get the role of the current user in the active organization

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val organizationId : kotlin.String = org_12345 // kotlin.String | Filter by organization ID
try {
    val result : GetActiveMemberRoleResponseDto = apiInstance.getActiveMemberRole(organizationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#getActiveMemberRole")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#getActiveMemberRole")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **organizationId** | **kotlin.String**| Filter by organization ID | [optional] |

### Return type

[**GetActiveMemberRoleResponseDto**](GetActiveMemberRoleResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getInvitation"></a>
# **getInvitation**
> GetInvitationResponseDto getInvitation(invitationId)

Get Invitation

Get an invitation by ID

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val invitationId : kotlin.String = inv_12345 // kotlin.String | The ID of the invitation to get
try {
    val result : GetInvitationResponseDto = apiInstance.getInvitation(invitationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#getInvitation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#getInvitation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **invitationId** | **kotlin.String**| The ID of the invitation to get | |

### Return type

[**GetInvitationResponseDto**](GetInvitationResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getOrganization"></a>
# **getOrganization**
> GetFullOrganizationResponseDto getOrganization(organizationId)

Get Full Organization

Get the full organization details

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val organizationId : kotlin.String = org_12345 // kotlin.String | The organization ID to get
try {
    val result : GetFullOrganizationResponseDto = apiInstance.getOrganization(organizationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#getOrganization")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#getOrganization")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **organizationId** | **kotlin.String**| The organization ID to get | [optional] |

### Return type

[**GetFullOrganizationResponseDto**](GetFullOrganizationResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
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

<a id="hasPermission"></a>
# **hasPermission**
> HasPermissionResponseDto hasPermission(hasPermissionDto)

Has Permission

Check if a user has permission

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val hasPermissionDto : HasPermissionDto =  // HasPermissionDto | 
try {
    val result : HasPermissionResponseDto = apiInstance.hasPermission(hasPermissionDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#hasPermission")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#hasPermission")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **hasPermissionDto** | [**HasPermissionDto**](HasPermissionDto.md)|  | |

### Return type

[**HasPermissionResponseDto**](HasPermissionResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="inviteMember"></a>
# **inviteMember**
> InviteMemberResponseDto inviteMember(inviteMemberDto)

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
    val result : InviteMemberResponseDto = apiInstance.inviteMember(inviteMemberDto)
    println(result)
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

[**InviteMemberResponseDto**](InviteMemberResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="leaveOrganization"></a>
# **leaveOrganization**
> LeaveOrganizationResponseDto leaveOrganization(leaveOrganizationDto)

Leave Organization

Leave an organization

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val leaveOrganizationDto : LeaveOrganizationDto =  // LeaveOrganizationDto | 
try {
    val result : LeaveOrganizationResponseDto = apiInstance.leaveOrganization(leaveOrganizationDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#leaveOrganization")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#leaveOrganization")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **leaveOrganizationDto** | [**LeaveOrganizationDto**](LeaveOrganizationDto.md)|  | |

### Return type

[**LeaveOrganizationResponseDto**](LeaveOrganizationResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="listApiKeys"></a>
# **listApiKeys**
> ListApiKeysResponseDto listApiKeys()

List API Keys

List all API keys for the current user

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
try {
    val result : ListApiKeysResponseDto = apiInstance.listApiKeys()
    println(result)
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

[**ListApiKeysResponseDto**](ListApiKeysResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listMembers"></a>
# **listMembers**
> ListMembersResponseDto listMembers(organizationId)

List Members

List all members of an organization

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val organizationId : kotlin.String = org_12345 // kotlin.String | Filter by organization ID
try {
    val result : ListMembersResponseDto = apiInstance.listMembers(organizationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#listMembers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#listMembers")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **organizationId** | **kotlin.String**| Filter by organization ID | [optional] |

### Return type

[**ListMembersResponseDto**](ListMembersResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listOrganizationInvitations"></a>
# **listOrganizationInvitations**
> ListInvitationsResponseDto listOrganizationInvitations(organizationId)

List Invitations

List all invitations a user has received

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val organizationId : kotlin.String = org_12345 // kotlin.String | Filter by organization ID
try {
    val result : ListInvitationsResponseDto = apiInstance.listOrganizationInvitations(organizationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#listOrganizationInvitations")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#listOrganizationInvitations")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **organizationId** | **kotlin.String**| Filter by organization ID | [optional] |

### Return type

[**ListInvitationsResponseDto**](ListInvitationsResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listOrganizations"></a>
# **listOrganizations**
> ListOrganizationsResponseDto listOrganizations(include)

List Organizations

List all organizations for the current user

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val include : kotlin.Boolean = true // kotlin.Boolean | Include additional organization data
try {
    val result : ListOrganizationsResponseDto = apiInstance.listOrganizations(include)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#listOrganizations")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#listOrganizations")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **include** | **kotlin.Boolean**| Include additional organization data | [optional] |

### Return type

[**ListOrganizationsResponseDto**](ListOrganizationsResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listUserInvitations"></a>
# **listUserInvitations**
> ListUserInvitationsResponseDto listUserInvitations(status)

List User Invitations

List all invitations a user has received

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val status : kotlin.String = pending // kotlin.String | Filter by status
try {
    val result : ListUserInvitationsResponseDto = apiInstance.listUserInvitations(status)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#listUserInvitations")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#listUserInvitations")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **status** | **kotlin.String**| Filter by status | [optional] |

### Return type

[**ListUserInvitationsResponseDto**](ListUserInvitationsResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listUserSessions"></a>
# **listUserSessions**
> ListSessionsResponseDto listUserSessions()

List User Sessions

List all active sessions for the user

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
try {
    val result : ListSessionsResponseDto = apiInstance.listUserSessions()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#listUserSessions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#listUserSessions")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListSessionsResponseDto**](ListSessionsResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="rejectInvitation"></a>
# **rejectInvitation**
> RejectInvitationResponseDto rejectInvitation(rejectInvitationDto)

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
    val result : RejectInvitationResponseDto = apiInstance.rejectInvitation(rejectInvitationDto)
    println(result)
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

[**RejectInvitationResponseDto**](RejectInvitationResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="removeMember"></a>
# **removeMember**
> RemoveMemberResponseDto removeMember(removeMemberDto)

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
    val result : RemoveMemberResponseDto = apiInstance.removeMember(removeMemberDto)
    println(result)
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

[**RemoveMemberResponseDto**](RemoveMemberResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="requestPasswordReset"></a>
# **requestPasswordReset**
> RequestPasswordResetResponseDto requestPasswordReset(requestPasswordResetDto)

Request Password Reset

Send a password reset email to the user

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val requestPasswordResetDto : RequestPasswordResetDto =  // RequestPasswordResetDto | 
try {
    val result : RequestPasswordResetResponseDto = apiInstance.requestPasswordReset(requestPasswordResetDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#requestPasswordReset")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#requestPasswordReset")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **requestPasswordResetDto** | [**RequestPasswordResetDto**](RequestPasswordResetDto.md)|  | |

### Return type

[**RequestPasswordResetResponseDto**](RequestPasswordResetResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="resetPassword"></a>
# **resetPassword**
> ResetPasswordResponseDto resetPassword(resetPasswordDto)

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
    val result : ResetPasswordResponseDto = apiInstance.resetPassword(resetPasswordDto)
    println(result)
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

[**ResetPasswordResponseDto**](ResetPasswordResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="resetPasswordCallback"></a>
# **resetPasswordCallback**
> ResetPasswordCallbackResponseDto resetPasswordCallback(token, callbackURL)

Reset Password Callback

Redirects user to callback URL with token

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val token : kotlin.String = token_example // kotlin.String | 
val callbackURL : kotlin.String = callbackURL_example // kotlin.String | 
try {
    val result : ResetPasswordCallbackResponseDto = apiInstance.resetPasswordCallback(token, callbackURL)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#resetPasswordCallback")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#resetPasswordCallback")
    e.printStackTrace()
}
```

### Parameters
| **token** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **callbackURL** | **kotlin.String**|  | |

### Return type

[**ResetPasswordCallbackResponseDto**](ResetPasswordCallbackResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="revokeSession"></a>
# **revokeSession**
> RevokeSessionResponseDto revokeSession(revokeSessionDto)

Revoke Session

Revoke a specific session

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val revokeSessionDto : RevokeSessionDto =  // RevokeSessionDto | 
try {
    val result : RevokeSessionResponseDto = apiInstance.revokeSession(revokeSessionDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#revokeSession")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#revokeSession")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **revokeSessionDto** | [**RevokeSessionDto**](RevokeSessionDto.md)|  | |

### Return type

[**RevokeSessionResponseDto**](RevokeSessionResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="sendVerificationEmail"></a>
# **sendVerificationEmail**
> SendVerificationEmailResponseDto sendVerificationEmail(sendVerificationEmailDto)

Send Verification Email

Send a verification email to the user

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val sendVerificationEmailDto : SendVerificationEmailDto =  // SendVerificationEmailDto | 
try {
    val result : SendVerificationEmailResponseDto = apiInstance.sendVerificationEmail(sendVerificationEmailDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#sendVerificationEmail")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#sendVerificationEmail")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sendVerificationEmailDto** | [**SendVerificationEmailDto**](SendVerificationEmailDto.md)|  | |

### Return type

[**SendVerificationEmailResponseDto**](SendVerificationEmailResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="setActiveOrganization"></a>
# **setActiveOrganization**
> SetActiveOrganizationResponseDto setActiveOrganization(setActiveOrganizationDto)

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
    val result : SetActiveOrganizationResponseDto = apiInstance.setActiveOrganization(setActiveOrganizationDto)
    println(result)
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

[**SetActiveOrganizationResponseDto**](SetActiveOrganizationResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="signInEmail"></a>
# **signInEmail**
> SignInResponseDto signInEmail(signInDto)

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
    val result : SignInResponseDto = apiInstance.signInEmail(signInDto)
    println(result)
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

[**SignInResponseDto**](SignInResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="signOut"></a>
# **signOut**
> SignOutResponseDto signOut()

Sign out

Sign out the current user and invalidate the session

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
try {
    val result : SignOutResponseDto = apiInstance.signOut()
    println(result)
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

[**SignOutResponseDto**](SignOutResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="signUpEmail"></a>
# **signUpEmail**
> SignUpResponseDto signUpEmail(signUpDto)

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
    val result : SignUpResponseDto = apiInstance.signUpEmail(signUpDto)
    println(result)
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

[**SignUpResponseDto**](SignUpResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="updateApiKey"></a>
# **updateApiKey**
> UpdateApiKeyResponseDto updateApiKey(updateApiKeyDto)

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
    val result : UpdateApiKeyResponseDto = apiInstance.updateApiKey(updateApiKeyDto)
    println(result)
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

[**UpdateApiKeyResponseDto**](UpdateApiKeyResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="updateMemberRole"></a>
# **updateMemberRole**
> UpdateMemberRoleResponseDto updateMemberRole(updateMemberRoleDto)

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
    val result : UpdateMemberRoleResponseDto = apiInstance.updateMemberRole(updateMemberRoleDto)
    println(result)
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

[**UpdateMemberRoleResponseDto**](UpdateMemberRoleResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="updateOrganization"></a>
# **updateOrganization**
> UpdateOrganizationResponseDto updateOrganization(updateOrganizationDto)

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
    val result : UpdateOrganizationResponseDto = apiInstance.updateOrganization(updateOrganizationDto)
    println(result)
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

[**UpdateOrganizationResponseDto**](UpdateOrganizationResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="updateUser"></a>
# **updateUser**
> UpdateUserResponseDto updateUser(updateUserDto)

Update User

Update the current user&#39;s information

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val updateUserDto : UpdateUserDto =  // UpdateUserDto | 
try {
    val result : UpdateUserResponseDto = apiInstance.updateUser(updateUserDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#updateUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#updateUser")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateUserDto** | [**UpdateUserDto**](UpdateUserDto.md)|  | |

### Return type

[**UpdateUserResponseDto**](UpdateUserResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="verifyApiKey"></a>
# **verifyApiKey**
> VerifyApiKeyResponseDto verifyApiKey(verifyApiKeyDto)

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
    val result : VerifyApiKeyResponseDto = apiInstance.verifyApiKey(verifyApiKeyDto)
    println(result)
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

[**VerifyApiKeyResponseDto**](VerifyApiKeyResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="verifyEmail"></a>
# **verifyEmail**
> VerifyEmailResponseDto verifyEmail(token, callbackURL)

Verify Email

Verify the email of a user

### Example
```kotlin
// Import classes:
//import com.cashful.kotlin.sdk.infrastructure.*
//import com.cashful.kotlin.sdk.model.*

val apiInstance = AuthenticationApi()
val token : kotlin.String = token_example // kotlin.String | 
val callbackURL : kotlin.String = callbackURL_example // kotlin.String | 
try {
    val result : VerifyEmailResponseDto = apiInstance.verifyEmail(token, callbackURL)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#verifyEmail")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#verifyEmail")
    e.printStackTrace()
}
```

### Parameters
| **token** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **callbackURL** | **kotlin.String**|  | [optional] |

### Return type

[**VerifyEmailResponseDto**](VerifyEmailResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

