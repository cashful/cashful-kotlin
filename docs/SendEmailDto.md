
# SendEmailDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **to** | [**kotlin.Any**](.md) | Recipient email address(es) |  |
| **subject** | **kotlin.String** | Email subject |  |
| **template** | **kotlin.String** | Template name to use (if using templates) |  [optional] |
| **context** | [**kotlin.Any**](.md) | Context variables for template rendering |  [optional] |
| **html** | **kotlin.String** | HTML content (if not using templates) |  [optional] |
| **text** | **kotlin.String** | Plain text content |  [optional] |
| **from** | **kotlin.String** | Sender email address |  [optional] |
| **cc** | [**kotlin.Any**](.md) | CC email address(es) |  [optional] |
| **bcc** | [**kotlin.Any**](.md) | BCC email address(es) |  [optional] |



