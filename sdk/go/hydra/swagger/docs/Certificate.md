# Certificate

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AuthorityKeyId** | **[]int32** |  | [optional] [default to null]
**BasicConstraintsValid** | **bool** | BasicConstraintsValid indicates whether IsCA, MaxPathLen, and MaxPathLenZero are valid. | [optional] [default to null]
**CRLDistributionPoints** | **[]string** | CRL Distribution Points | [optional] [default to null]
**DNSNames** | **[]string** | Subject Alternate Name values. (Note that these values may not be valid if invalid values were contained within a parsed certificate. For example, an element of DNSNames may not be a valid DNS domain name.) | [optional] [default to null]
**EmailAddresses** | **[]string** |  | [optional] [default to null]
**ExcludedDNSDomains** | **[]string** |  | [optional] [default to null]
**ExcludedEmailAddresses** | **[]string** |  | [optional] [default to null]
**ExcludedIPRanges** | [**[]IpNet**](IPNet.md) |  | [optional] [default to null]
**ExcludedURIDomains** | **[]string** |  | [optional] [default to null]
**ExtKeyUsage** | [**[]ExtKeyUsage**](ExtKeyUsage.md) |  | [optional] [default to null]
**Extensions** | [**[]Extension**](Extension.md) | Extensions contains raw X.509 extensions. When parsing certificates, this can be used to extract non-critical extensions that are not parsed by this package. When marshaling certificates, the Extensions field is ignored, see ExtraExtensions. | [optional] [default to null]
**ExtraExtensions** | [**[]Extension**](Extension.md) | ExtraExtensions contains extensions to be copied, raw, into any marshaled certificates. Values override any extensions that would otherwise be produced based on the other fields. The ExtraExtensions field is not populated when parsing certificates, see Extensions. | [optional] [default to null]
**IPAddresses** | [**[]Ip**](IP.md) |  | [optional] [default to null]
**IsCA** | **bool** |  | [optional] [default to null]
**Issuer** | [**Name**](Name.md) |  | [optional] [default to null]
**IssuingCertificateURL** | **[]string** |  | [optional] [default to null]
**KeyUsage** | [**KeyUsage**](KeyUsage.md) |  | [optional] [default to null]
**MaxPathLen** | **int64** | MaxPathLen and MaxPathLenZero indicate the presence and value of the BasicConstraints&#39; \&quot;pathLenConstraint\&quot;.  When parsing a certificate, a positive non-zero MaxPathLen means that the field was specified, -1 means it was unset, and MaxPathLenZero being true mean that the field was explicitly set to zero. The case of MaxPathLen&#x3D;&#x3D;0 with MaxPathLenZero&#x3D;&#x3D;false should be treated equivalent to -1 (unset).  When generating a certificate, an unset pathLenConstraint can be requested with either MaxPathLen &#x3D;&#x3D; -1 or using the zero value for both MaxPathLen and MaxPathLenZero. | [optional] [default to null]
**MaxPathLenZero** | **bool** | MaxPathLenZero indicates that BasicConstraintsValid&#x3D;&#x3D;true and MaxPathLen&#x3D;&#x3D;0 should be interpreted as an actual maximum path length of zero. Otherwise, that combination is interpreted as MaxPathLen not being set. | [optional] [default to null]
**NotBefore** | [**time.Time**](time.Time.md) |  | [optional] [default to null]
**OCSPServer** | **[]string** | RFC 5280, 4.2.2.1 (Authority Information Access) | [optional] [default to null]
**PermittedDNSDomains** | **[]string** |  | [optional] [default to null]
**PermittedDNSDomainsCritical** | **bool** | Name constraints | [optional] [default to null]
**PermittedEmailAddresses** | **[]string** |  | [optional] [default to null]
**PermittedIPRanges** | [**[]IpNet**](IPNet.md) |  | [optional] [default to null]
**PermittedURIDomains** | **[]string** |  | [optional] [default to null]
**PolicyIdentifiers** | [**[]ObjectIdentifier**](ObjectIdentifier.md) |  | [optional] [default to null]
**PublicKey** | [**interface{}**](interface{}.md) |  | [optional] [default to null]
**PublicKeyAlgorithm** | [**PublicKeyAlgorithm**](PublicKeyAlgorithm.md) |  | [optional] [default to null]
**Raw** | **[]int32** |  | [optional] [default to null]
**RawIssuer** | **[]int32** |  | [optional] [default to null]
**RawSubject** | **[]int32** |  | [optional] [default to null]
**RawSubjectPublicKeyInfo** | **[]int32** |  | [optional] [default to null]
**RawTBSCertificate** | **[]int32** |  | [optional] [default to null]
**SerialNumber** | [**ModelInt**](Int.md) |  | [optional] [default to null]
**Signature** | **[]int32** |  | [optional] [default to null]
**SignatureAlgorithm** | [**SignatureAlgorithm**](SignatureAlgorithm.md) |  | [optional] [default to null]
**Subject** | [**Name**](Name.md) |  | [optional] [default to null]
**SubjectKeyId** | **[]int32** |  | [optional] [default to null]
**URIs** | [**[]Url**](URL.md) |  | [optional] [default to null]
**UnhandledCriticalExtensions** | [**[]ObjectIdentifier**](ObjectIdentifier.md) | UnhandledCriticalExtensions contains a list of extension IDs that were not (fully) processed when parsing. Verify will fail if this slice is non-empty, unless verification is delegated to an OS library which understands all the critical extensions.  Users can access these extensions using Extensions and can remove elements from this slice if they believe that they have been handled. | [optional] [default to null]
**UnknownExtKeyUsage** | [**[]ObjectIdentifier**](ObjectIdentifier.md) |  | [optional] [default to null]
**Version** | **int64** |  | [optional] [default to null]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


