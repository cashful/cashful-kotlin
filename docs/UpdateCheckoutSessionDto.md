
# UpdateCheckoutSessionDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **status** | **kotlin.String** |  |  |
| **metadata** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) | Optional custom metadata |  |
| **successUrl** | **kotlin.String** | The URL to redirect to on successful payment |  [optional] |
| **failureUrl** | **kotlin.String** | The URL to redirect to on failure |  [optional] |
| **cancelUrl** | **kotlin.String** | The URL to redirect to on cancel |  [optional] |
| **hostedCheckoutConfig** | [**HostedCheckoutConfigDto**](HostedCheckoutConfigDto.md) | Configuration for the hosted checkout page |  [optional] |



