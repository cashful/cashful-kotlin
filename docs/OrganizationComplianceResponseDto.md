
# OrganizationComplianceResponseDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | Unique identifier |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  |
| **organizationId** | **kotlin.String** |  |  |
| **deletedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **companyRegistrationName** | **kotlin.String** |  |  [optional] |
| **companyRegistrationNumber** | **kotlin.String** |  |  [optional] |
| **companyTradingName** | **kotlin.String** |  |  [optional] |
| **vatRegistrationNumber** | **kotlin.String** |  |  [optional] |
| **industry** | **kotlin.String** |  |  [optional] |
| **subIndustry** | **kotlin.String** |  |  [optional] |
| **estimatedAnnualTurnover** | **kotlin.String** |  |  [optional] |
| **businessDescription** | **kotlin.String** |  |  [optional] |
| **companyMobileMoneySettlementNumber** | **kotlin.String** |  |  [optional] |
| **companyEmail** | **kotlin.String** |  |  [optional] |
| **companyContactNumber** | **kotlin.String** |  |  [optional] |
| **website** | **kotlin.String** |  |  [optional] |
| **socialMedia** | **kotlin.String** |  |  [optional] |
| **accountContactNumber** | **kotlin.String** |  |  [optional] |
| **customerSupportContactNumber** | **kotlin.String** |  |  [optional] |
| **customerSupportEscalationContactNumber** | **kotlin.String** |  |  [optional] |
| **emergencyContactNumber** | **kotlin.String** |  |  [optional] |
| **streetAddress** | **kotlin.String** |  |  [optional] |
| **apartment** | **kotlin.String** |  |  [optional] |
| **suburb** | **kotlin.String** |  |  [optional] |
| **city** | **kotlin.String** |  |  [optional] |
| **postalCode** | **kotlin.String** |  |  [optional] |
| **country** | **kotlin.String** |  |  [optional] |
| **bank** | **kotlin.String** |  |  [optional] |
| **accountType** | **kotlin.String** |  |  [optional] |
| **accountName** | **kotlin.String** |  |  [optional] |
| **accountNumber** | **kotlin.String** |  |  [optional] |
| **branchCode** | **kotlin.String** |  |  [optional] |
| **swiftCode** | **kotlin.String** |  |  [optional] |
| **certificateOfIncorporation** | **kotlin.String** |  |  [optional] |
| **identityDocuments** | **kotlin.String** |  |  [optional] |
| **bankAccountConfirmationLetter** | **kotlin.String** |  |  [optional] |
| **proofOfBusinessAddress** | **kotlin.String** |  |  [optional] |
| **termsAccepted** | **kotlin.Boolean** |  |  [optional] |
| **acceptedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **currentStep** | [**inline**](#CurrentStep) |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **isCompleted** | **kotlin.Boolean** |  |  [optional] |
| **completionScore** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |


<a id="CurrentStep"></a>
## Enum: currentStep
| Name | Value |
| ---- | ----- |
| currentStep | initiation, verification, business_details, banking_details, upload_documents, sign_agreement |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | pending, verified, rejected |



