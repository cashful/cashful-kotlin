
# JwkDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **kid** | **kotlin.String** | Key ID uniquely identifying the key |  |
| **kty** | **kotlin.String** | Key type (e.g., &#39;RSA&#39;, &#39;EC&#39;, &#39;OKP&#39;) |  |
| **alg** | **kotlin.String** | Algorithm intended for use with the key |  |
| **use** | [**inline**](#Use) | Intended use of the public key |  [optional] |
| **n** | **kotlin.String** | Modulus for RSA keys |  [optional] |
| **e** | **kotlin.String** | Exponent for RSA keys |  [optional] |
| **crv** | **kotlin.String** | Curve name for elliptic curve keys |  [optional] |
| **x** | **kotlin.String** | X coordinate for elliptic curve keys |  [optional] |
| **y** | **kotlin.String** | Y coordinate for elliptic curve keys |  [optional] |


<a id="Use"></a>
## Enum: use
| Name | Value |
| ---- | ----- |
| use | sig |



