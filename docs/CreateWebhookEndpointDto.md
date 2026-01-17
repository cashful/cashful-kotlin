
# CreateWebhookEndpointDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **url** | **kotlin.String** | The URL where webhook events will be sent |  |
| **events** | **kotlin.collections.List&lt;kotlin.String&gt;** | Array of event types to listen for |  |
| **merchantId** | **kotlin.String** | The ID of the merchant whose balance is being requested. If omitted, defaults to the authenticated merchant. |  [optional] |
| **metadata** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) | Optional custom metadata |  [optional] |



