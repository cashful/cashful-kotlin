# AuthenticationApi

All URIs are relative to *https://api.cashful.africa*

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
| [**getAccessToken**](AuthenticationApi.md#getAccessToken) | **POST** /api/canary/authentication/get-access-token | Get Access Token |
| [**getActiveMember**](AuthenticationApi.md#getActiveMember) | **GET** /api/canary/authentication/organization/get-active-member | Get Active Member |
| [**getActiveMemberRole**](AuthenticationApi.md#getActiveMemberRole) | **GET** /api/canary/authentication/organization/get-active-member-role | Get Active Member Role |
| [**getApiKey**](AuthenticationApi.md#getApiKey) | **GET** /api/canary/authentication/api-key/get | Get API Key |
| [**getInvitation**](AuthenticationApi.md#getInvitation) | **GET** /api/canary/authentication/organization/get-invitation | Get Invitation |
| [**getOrganization**](AuthenticationApi.md#getOrganization) | **GET** /api/canary/authentication/organization/get-full-organization | Get Full Organization |
| [**getSession**](AuthenticationApi.md#getSession) | **GET** /api/canary/authentication/get-session | Get Session |
| [**hasPermission**](AuthenticationApi.md#hasPermission) | **POST** /api/canary/authentication/organization/has-permission | Has Permission |
| [**inviteMember**](AuthenticationApi.md#inviteMember) | **POST** /api/canary/authentication/organization/invite-member | Invite Member |
| [**isUsernameAvailable**](AuthenticationApi.md#isUsernameAvailable) | **POST** /api/canary/authentication/is-username-available | Check Username Availability |
| [**leaveOrganization**](AuthenticationApi.md#leaveOrganization) | **POST** /api/canary/authentication/organization/leave | Leave Organization |
| [**linkSocial**](AuthenticationApi.md#linkSocial) | **POST** /api/canary/authentication/link-social | Link Social Account |
| [**listAccounts**](AuthenticationApi.md#listAccounts) | **GET** /api/canary/authentication/list-accounts | List Linked Accounts |
| [**listApiKeys**](AuthenticationApi.md#listApiKeys) | **GET** /api/canary/authentication/api-key/list | List API Keys |
| [**listMembers**](AuthenticationApi.md#listMembers) | **GET** /api/canary/authentication/organization/list-members | List Members |
| [**listOrganizationInvitations**](AuthenticationApi.md#listOrganizationInvitations) | **GET** /api/canary/authentication/organization/list-invitations | List Invitations |
| [**listOrganizations**](AuthenticationApi.md#listOrganizations) | **GET** /api/canary/authentication/organization/list | List Organizations |
| [**listUserInvitations**](AuthenticationApi.md#listUserInvitations) | **GET** /api/canary/authentication/organization/list-user-invitations | List User Invitations |
| [**listUserSessions**](AuthenticationApi.md#listUserSessions) | **GET** /api/canary/authentication/list-sessions | List User Sessions |
| [**ok**](AuthenticationApi.md#ok) | **GET** /api/canary/authentication/ok | Health Check |
| [**refreshToken**](AuthenticationApi.md#refreshToken) | **POST** /api/canary/authentication/refresh-token | Refresh Token |
| [**rejectInvitation**](AuthenticationApi.md#rejectInvitation) | **POST** /api/canary/authentication/organization/reject-invitation | Reject Invitation |
| [**removeMember**](AuthenticationApi.md#removeMember) | **POST** /api/canary/authentication/organization/remove-member | Remove Member |
| [**requestPasswordReset**](AuthenticationApi.md#requestPasswordReset) | **POST** /api/canary/authentication/request-password-reset | Request Password Reset |
| [**requestPhonePasswordReset**](AuthenticationApi.md#requestPhonePasswordReset) | **POST** /api/canary/authentication/phone-number/request-password-reset | Request Password Reset via Phone |
| [**resetPassword**](AuthenticationApi.md#resetPassword) | **POST** /api/canary/authentication/reset-password | Reset Password |
| [**resetPasswordCallback**](AuthenticationApi.md#resetPasswordCallback) | **GET** /api/canary/authentication/reset-password/{token} | Reset Password Callback |
| [**resetPhonePassword**](AuthenticationApi.md#resetPhonePassword) | **POST** /api/canary/authentication/phone-number/reset-password | Reset Password with Phone |
| [**revokeOtherSessions**](AuthenticationApi.md#revokeOtherSessions) | **POST** /api/canary/authentication/revoke-other-sessions | Revoke Other Sessions |
| [**revokeSession**](AuthenticationApi.md#revokeSession) | **POST** /api/canary/authentication/revoke-session | Revoke Session |
| [**revokeSessions**](AuthenticationApi.md#revokeSessions) | **POST** /api/canary/authentication/revoke-sessions | Revoke All Sessions |
| [**sendPhoneOTP**](AuthenticationApi.md#sendPhoneOTP) | **POST** /api/canary/authentication/phone-number/send-otp | Send OTP to Phone |
| [**sendVerificationEmail**](AuthenticationApi.md#sendVerificationEmail) | **POST** /api/canary/authentication/send-verification-email | Send Verification Email |
| [**setActiveOrganization**](AuthenticationApi.md#setActiveOrganization) | **POST** /api/canary/authentication/organization/set-active | Set Active Organization |
| [**signInEmail**](AuthenticationApi.md#signInEmail) | **POST** /api/canary/authentication/sign-in/email | Sign in with email |
| [**signInPhoneNumber**](AuthenticationApi.md#signInPhoneNumber) | **POST** /api/canary/authentication/sign-in/phone-number | Sign in with Phone Number |
| [**signOut**](AuthenticationApi.md#signOut) | **POST** /api/canary/authentication/sign-out | Sign out |
| [**signUpEmail**](AuthenticationApi.md#signUpEmail) | **POST** /api/canary/authentication/sign-up/email | Sign up with email |
| [**socialSignIn**](AuthenticationApi.md#socialSignIn) | **POST** /api/canary/authentication/sign-in/social | Sign in with social provider |
| [**unlinkAccount**](AuthenticationApi.md#unlinkAccount) | **POST** /api/canary/authentication/unlink-account | Unlink Social Account |
| [**updateApiKey**](AuthenticationApi.md#updateApiKey) | **POST** /api/canary/authentication/api-key/update | Update API Key |
| [**updateMemberRole**](AuthenticationApi.md#updateMemberRole) | **POST** /api/canary/authentication/organization/update-member-role | Update Member Role |
| [**updateOrganization**](AuthenticationApi.md#updateOrganization) | **POST** /api/canary/authentication/organization/update | Update Organization |
| [**updateUser**](AuthenticationApi.md#updateUser) | **POST** /api/canary/authentication/update-user | Update User |
| [**verifyApiKey**](AuthenticationApi.md#verifyApiKey) | **POST** /api/canary/authentication/api-key/verify | Verify API Key |
| [**verifyEmail**](AuthenticationApi.md#verifyEmail) | **GET** /api/canary/authentication/verify-email | Verify Email |
| [**verifyPhoneNumber**](AuthenticationApi.md#verifyPhoneNumber) | **POST** /api/canary/authentication/phone-number/verify | Verify Phone Number |


<a id="acceptInvitation"></a>
# **acceptInvitation**
> AcceptInvitationResponseDto acceptInvitation(acceptInvitationDto)

Accept Invitation

Accept an invitation to an organization

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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

<a id="getAccessToken"></a>
# **getAccessToken**
> GetAccessTokenResponseDto getAccessToken(getAccessTokenDto)

Get Access Token

Get current access token

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AuthenticationApi()
val getAccessTokenDto : GetAccessTokenDto =  // GetAccessTokenDto | 
try {
    val result : GetAccessTokenResponseDto = apiInstance.getAccessToken(getAccessTokenDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#getAccessToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#getAccessToken")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **getAccessTokenDto** | [**GetAccessTokenDto**](GetAccessTokenDto.md)|  | |

### Return type

[**GetAccessTokenResponseDto**](GetAccessTokenResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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

<a id="getApiKey"></a>
# **getApiKey**
> GetApiKeyResponseDto getApiKey(id)

Get API Key

Retrieve a specific API key by ID

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AuthenticationApi()
val id : kotlin.String = key_12345 // kotlin.String | The ID of API key to retrieve
try {
    val result : GetApiKeyResponseDto = apiInstance.getApiKey(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#getApiKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#getApiKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The ID of API key to retrieve | |

### Return type

[**GetApiKeyResponseDto**](GetApiKeyResponseDto.md)

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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

<a id="isUsernameAvailable"></a>
# **isUsernameAvailable**
> IsUsernameAvailableResponseDto isUsernameAvailable(isUsernameAvailableDto)

Check Username Availability

Check if username is available for signup

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AuthenticationApi()
val isUsernameAvailableDto : IsUsernameAvailableDto =  // IsUsernameAvailableDto | 
try {
    val result : IsUsernameAvailableResponseDto = apiInstance.isUsernameAvailable(isUsernameAvailableDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#isUsernameAvailable")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#isUsernameAvailable")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **isUsernameAvailableDto** | [**IsUsernameAvailableDto**](IsUsernameAvailableDto.md)|  | |

### Return type

[**IsUsernameAvailableResponseDto**](IsUsernameAvailableResponseDto.md)

### Authorization

No authorization required

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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

<a id="linkSocial"></a>
# **linkSocial**
> LinkSocialResponseDto linkSocial(linkSocialDto)

Link Social Account

Link a social account to existing user

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AuthenticationApi()
val linkSocialDto : LinkSocialDto =  // LinkSocialDto | 
try {
    val result : LinkSocialResponseDto = apiInstance.linkSocial(linkSocialDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#linkSocial")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#linkSocial")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **linkSocialDto** | [**LinkSocialDto**](LinkSocialDto.md)|  | |

### Return type

[**LinkSocialResponseDto**](LinkSocialResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="listAccounts"></a>
# **listAccounts**
> ListAccountsResponseDto listAccounts()

List Linked Accounts

List all linked social accounts

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AuthenticationApi()
try {
    val result : ListAccountsResponseDto = apiInstance.listAccounts()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#listAccounts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#listAccounts")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListAccountsResponseDto**](ListAccountsResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listApiKeys"></a>
# **listApiKeys**
> ListApiKeysResponseDto listApiKeys()

List API Keys

List all API keys for the current user

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
> kotlin.collections.List&lt;OrganizationDto&gt; listOrganizations(include)

List Organizations

List all organizations for the current user

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AuthenticationApi()
val include : kotlin.Boolean = true // kotlin.Boolean | Include additional organization data
try {
    val result : kotlin.collections.List<OrganizationDto> = apiInstance.listOrganizations(include)
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

[**kotlin.collections.List&lt;OrganizationDto&gt;**](OrganizationDto.md)

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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

<a id="ok"></a>
# **ok**
> kotlin.String ok()

Health Check

Check if the authentication API is working

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AuthenticationApi()
try {
    val result : kotlin.String = apiInstance.ok()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#ok")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#ok")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**kotlin.String**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="refreshToken"></a>
# **refreshToken**
> RefreshTokenResponseDto refreshToken(refreshTokenDto)

Refresh Token

Refresh authentication token

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AuthenticationApi()
val refreshTokenDto : RefreshTokenDto =  // RefreshTokenDto | 
try {
    val result : RefreshTokenResponseDto = apiInstance.refreshToken(refreshTokenDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#refreshToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#refreshToken")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **refreshTokenDto** | [**RefreshTokenDto**](RefreshTokenDto.md)|  | |

### Return type

[**RefreshTokenResponseDto**](RefreshTokenResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="rejectInvitation"></a>
# **rejectInvitation**
> RejectInvitationResponseDto rejectInvitation(rejectInvitationDto)

Reject Invitation

Reject an invitation to an organization

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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

<a id="requestPhonePasswordReset"></a>
# **requestPhonePasswordReset**
> RequestPhonePasswordResetResponseDto requestPhonePasswordReset(requestPhonePasswordResetDto)

Request Password Reset via Phone

Request password reset via phone number

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AuthenticationApi()
val requestPhonePasswordResetDto : RequestPhonePasswordResetDto =  // RequestPhonePasswordResetDto | 
try {
    val result : RequestPhonePasswordResetResponseDto = apiInstance.requestPhonePasswordReset(requestPhonePasswordResetDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#requestPhonePasswordReset")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#requestPhonePasswordReset")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **requestPhonePasswordResetDto** | [**RequestPhonePasswordResetDto**](RequestPhonePasswordResetDto.md)|  | |

### Return type

[**RequestPhonePasswordResetResponseDto**](RequestPhonePasswordResetResponseDto.md)

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AuthenticationApi()
val token : kotlin.String = token_example // kotlin.String | 
val callbackURL : kotlin.String = https://example.com/reset-password // kotlin.String | The URL to redirect user to reset their password
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
| **callbackURL** | **kotlin.String**| The URL to redirect user to reset their password | |

### Return type

[**ResetPasswordCallbackResponseDto**](ResetPasswordCallbackResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="resetPhonePassword"></a>
# **resetPhonePassword**
> ResetPhonePasswordResponseDto resetPhonePassword(resetPhonePasswordDto)

Reset Password with Phone

Reset password using phone verification

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AuthenticationApi()
val resetPhonePasswordDto : ResetPhonePasswordDto =  // ResetPhonePasswordDto | 
try {
    val result : ResetPhonePasswordResponseDto = apiInstance.resetPhonePassword(resetPhonePasswordDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#resetPhonePassword")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#resetPhonePassword")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **resetPhonePasswordDto** | [**ResetPhonePasswordDto**](ResetPhonePasswordDto.md)|  | |

### Return type

[**ResetPhonePasswordResponseDto**](ResetPhonePasswordResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="revokeOtherSessions"></a>
# **revokeOtherSessions**
> RevokeSessionResponseDto revokeOtherSessions()

Revoke Other Sessions

Revoke all sessions except the current one

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AuthenticationApi()
try {
    val result : RevokeSessionResponseDto = apiInstance.revokeOtherSessions()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#revokeOtherSessions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#revokeOtherSessions")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**RevokeSessionResponseDto**](RevokeSessionResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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

<a id="revokeSessions"></a>
# **revokeSessions**
> RevokeSessionResponseDto revokeSessions()

Revoke All Sessions

Revoke all sessions for the current user

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AuthenticationApi()
try {
    val result : RevokeSessionResponseDto = apiInstance.revokeSessions()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#revokeSessions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#revokeSessions")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**RevokeSessionResponseDto**](RevokeSessionResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="sendPhoneOTP"></a>
# **sendPhoneOTP**
> SendPhoneOTPResponseDto sendPhoneOTP(sendPhoneOTPDto)

Send OTP to Phone

Send one-time password to phone number

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AuthenticationApi()
val sendPhoneOTPDto : SendPhoneOTPDto =  // SendPhoneOTPDto | 
try {
    val result : SendPhoneOTPResponseDto = apiInstance.sendPhoneOTP(sendPhoneOTPDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#sendPhoneOTP")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#sendPhoneOTP")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sendPhoneOTPDto** | [**SendPhoneOTPDto**](SendPhoneOTPDto.md)|  | |

### Return type

[**SendPhoneOTPResponseDto**](SendPhoneOTPResponseDto.md)

### Authorization

No authorization required

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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

<a id="signInPhoneNumber"></a>
# **signInPhoneNumber**
> SignInResponseDto signInPhoneNumber(signInPhoneNumberDto)

Sign in with Phone Number

Sign in using phone number and password

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AuthenticationApi()
val signInPhoneNumberDto : SignInPhoneNumberDto =  // SignInPhoneNumberDto | 
try {
    val result : SignInResponseDto = apiInstance.signInPhoneNumber(signInPhoneNumberDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#signInPhoneNumber")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#signInPhoneNumber")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **signInPhoneNumberDto** | [**SignInPhoneNumberDto**](SignInPhoneNumberDto.md)|  | |

### Return type

[**SignInResponseDto**](SignInResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="signOut"></a>
# **signOut**
> SignOutResponseDto signOut(body)

Sign out

Sign out the current user and invalidate the session

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AuthenticationApi()
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : SignOutResponseDto = apiInstance.signOut(body)
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
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

### Return type

[**SignOutResponseDto**](SignOutResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="signUpEmail"></a>
# **signUpEmail**
> SignUpResponseDto signUpEmail(signUpDto)

Sign up with email

Create a new user account using email and password

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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

<a id="socialSignIn"></a>
# **socialSignIn**
> SignInResponseDto socialSignIn(socialSignInDto)

Sign in with social provider

Sign in with a social provider (OAuth, etc.)

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AuthenticationApi()
val socialSignInDto : SocialSignInDto =  // SocialSignInDto | 
try {
    val result : SignInResponseDto = apiInstance.socialSignIn(socialSignInDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#socialSignIn")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#socialSignIn")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **socialSignInDto** | [**SocialSignInDto**](SocialSignInDto.md)|  | |

### Return type

[**SignInResponseDto**](SignInResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="unlinkAccount"></a>
# **unlinkAccount**
> UnlinkAccountResponseDto unlinkAccount(unlinkAccountDto)

Unlink Social Account

Unlink a social account from user

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AuthenticationApi()
val unlinkAccountDto : UnlinkAccountDto =  // UnlinkAccountDto | 
try {
    val result : UnlinkAccountResponseDto = apiInstance.unlinkAccount(unlinkAccountDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#unlinkAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#unlinkAccount")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **unlinkAccountDto** | [**UnlinkAccountDto**](UnlinkAccountDto.md)|  | |

### Return type

[**UnlinkAccountResponseDto**](UnlinkAccountResponseDto.md)

### Authorization


Configure bearer:
    ApiClient.accessToken = ""

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

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
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AuthenticationApi()
val token : kotlin.String = verify_token_12345 // kotlin.String | The token to verify email
val callbackURL : kotlin.String = https://example.com/callback // kotlin.String | The URL to redirect to after email verification
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
| **token** | **kotlin.String**| The token to verify email | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **callbackURL** | **kotlin.String**| The URL to redirect to after email verification | [optional] |

### Return type

[**VerifyEmailResponseDto**](VerifyEmailResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="verifyPhoneNumber"></a>
# **verifyPhoneNumber**
> VerifyPhoneNumberResponseDto verifyPhoneNumber(verifyPhoneNumberDto)

Verify Phone Number

Verify phone number with OTP code

### Example
```kotlin
// Import classes:
//import com.cashful.infrastructure.*
//import com.cashful.model.*

val apiInstance = AuthenticationApi()
val verifyPhoneNumberDto : VerifyPhoneNumberDto =  // VerifyPhoneNumberDto | 
try {
    val result : VerifyPhoneNumberResponseDto = apiInstance.verifyPhoneNumber(verifyPhoneNumberDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthenticationApi#verifyPhoneNumber")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthenticationApi#verifyPhoneNumber")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **verifyPhoneNumberDto** | [**VerifyPhoneNumberDto**](VerifyPhoneNumberDto.md)|  | |

### Return type

[**VerifyPhoneNumberResponseDto**](VerifyPhoneNumberResponseDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

