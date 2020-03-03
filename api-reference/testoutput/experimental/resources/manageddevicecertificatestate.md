---
title: "managedDeviceCertificateState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedDeviceCertificateState resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List managedDeviceCertificateStates](../api/manageddevicecertificatestate-list.md)|[managedDeviceCertificateState](../resources/manageddevicecertificatestate.md) collection|List properties and relationships of the [managedDeviceCertificateState](../resources/manageddevicecertificatestate.md) objects.|
|[Get managedDeviceCertificateState](../api/manageddevicecertificatestate-get.md)|[managedDeviceCertificateState](../resources/manageddevicecertificatestate.md)|Read properties and relationships of the [managedDeviceCertificateState](../resources/manageddevicecertificatestate.md) object.|
|[Create managedDeviceCertificateState](../api/manageddevicecertificatestate-create.md)|[managedDeviceCertificateState](../resources/manageddevicecertificatestate.md)|Create a new [managedDeviceCertificateState](../resources/manageddevicecertificatestate.md) object.|
|[Delete managedDeviceCertificateState](../api/manageddevicecertificatestate-delete.md)|None|Deletes a [managedDeviceCertificateState](../resources/manageddevicecertificatestate.md).|
|[Update managedDeviceCertificateState](../api/manageddevicecertificatestate-update.md)|[managedDeviceCertificateState](../resources/manageddevicecertificatestate.md)|Update the properties of a [managedDeviceCertificateState](../resources/manageddevicecertificatestate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|certificateEnhancedKeyUsage|String|Extended key usage|
|certificateErrorCode|Int32|Error code|
|certificateExpirationDateTime|DateTimeOffset|Certificate expiry date|
|certificateIssuanceDateTime|DateTimeOffset|Issuance date|
|certificateIssuanceState|Enumeration|Issuance State. Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.|
|certificateIssuer|String|Issuer|
|certificateKeyLength|Int32|Key length|
|certificateKeyStorageProvider|Enumeration|Key Storage Provider. Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.|
|certificateKeyUsage|Enumeration|Key usage. Possible values are: `keyEncipherment`, `digitalSignature`.|
|certificateLastIssuanceStateChangedDateTime|DateTimeOffset|Last certificate issuance state change|
|certificateProfileDisplayName|String|Certificate profile display name|
|certificateRevokeStatus|Enumeration|Revoke status. Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.|
|certificateSerialNumber|String|Serial number|
|certificateSubjectAlternativeNameFormat|Enumeration|Subject alternative name format. Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.|
|certificateSubjectAlternativeNameFormatString|String|Subject alternative name format string for custom formats|
|certificateSubjectNameFormat|Enumeration|Subject name format. Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|certificateSubjectNameFormatString|String|Subject name format string for custom subject name formats|
|certificateThumbprint|String|Thumbprint|
|certificateValidityPeriod|Int32|Validity period|
|certificateValidityPeriodUnits|Enumeration|Validity period units. Possible values are: `days`, `months`, `years`.|
|deviceDisplayName|String|Device display name|
|devicePlatform|Enumeration|Device platform. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastCertificateStateChangeDateTime|DateTimeOffset|Last certificate issuance state change|
|userDisplayName|String|User display name|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceCertificateState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
  "id": "String (identifier)",
  "devicePlatform": "String",
  "certificateKeyUsage": "String",
  "certificateValidityPeriodUnits": "String",
  "certificateIssuanceState": "String",
  "certificateKeyStorageProvider": "String",
  "certificateSubjectNameFormat": "String",
  "certificateSubjectAlternativeNameFormat": "String",
  "certificateRevokeStatus": "String",
  "certificateProfileDisplayName": "String",
  "deviceDisplayName": "String",
  "userDisplayName": "String",
  "certificateExpirationDateTime": "String (timestamp)",
  "certificateLastIssuanceStateChangedDateTime": "String (timestamp)",
  "lastCertificateStateChangeDateTime": "String (timestamp)",
  "certificateIssuer": "String",
  "certificateThumbprint": "String",
  "certificateSerialNumber": "String",
  "certificateKeyLength": 1024,
  "certificateEnhancedKeyUsage": "String",
  "certificateValidityPeriod": 1024,
  "certificateSubjectNameFormatString": "String",
  "certificateSubjectAlternativeNameFormatString": "String",
  "certificateIssuanceDateTime": "String (timestamp)",
  "certificateErrorCode": 1024
}
```

