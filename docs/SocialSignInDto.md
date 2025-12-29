
# SocialSignInDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **provider** | **kotlin.String** | The social provider to sign in with |  |
| **callbackURL** | **kotlin.String** | Callback URL to redirect to after the user has signed in |  [optional] |
| **newUserCallbackURL** | **kotlin.String** | Callback URL for new users |  [optional] |
| **errorCallbackURL** | **kotlin.String** | Callback URL for errors |  [optional] |
| **disableRedirect** | **kotlin.Boolean** | Disable automatic redirection to the provider |  [optional] |
| **idToken** | [**kotlin.Any**](.md) | ID token from provider |  [optional] |
| **scopes** | **kotlin.collections.List&lt;kotlin.String&gt;** | Array of scopes to request from the provider |  [optional] |
| **requestSignUp** | **kotlin.Boolean** | Explicitly request sign-up |  [optional] |
| **loginHint** | **kotlin.String** | Login hint for the authorization code request |  [optional] |
| **additionalData** | **kotlin.String** | Additional data for the request |  [optional] |



