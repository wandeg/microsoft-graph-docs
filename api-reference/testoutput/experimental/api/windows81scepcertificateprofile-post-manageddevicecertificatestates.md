---
title: "Create managedDeviceCertificateStates"
description: "Create managedDeviceCertificateStates by posting to the managedDeviceCertificateStates collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create managedDeviceCertificateStates

Namespace: microsoft.graph

Create managedDeviceCertificateStates by posting to the managedDeviceCertificateStates collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [managedDeviceCertificateState](../resources/manageddevicecertificatestate.md) object.

The following table shows the properties that are required when you create the [managedDeviceCertificateState](../resources/manageddevicecertificatestate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|devicePlatform|Enumeration|Device platform. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|certificateKeyUsage|Enumeration|Key usage. Possible values are: `keyEncipherment`, `digitalSignature`.|
|certificateValidityPeriodUnits|Enumeration|Validity period units. Possible values are: `days`, `months`, `years`.|
|certificateIssuanceState|Enumeration|Issuance State. Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.|
|certificateKeyStorageProvider|Enumeration|Key Storage Provider. Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.|
|certificateSubjectNameFormat|Enumeration|Subject name format. Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|certificateSubjectAlternativeNameFormat|Enumeration|Subject alternative name format. Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.|
|certificateRevokeStatus|Enumeration|Revoke status. Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.|
|certificateProfileDisplayName|String|Certificate profile display name|
|deviceDisplayName|String|Device display name|
|userDisplayName|String|User display name|
|certificateExpirationDateTime|DateTimeOffset|Certificate expiry date|
|certificateLastIssuanceStateChangedDateTime|DateTimeOffset|Last certificate issuance state change|
|lastCertificateStateChangeDateTime|DateTimeOffset|Last certificate issuance state change|
|certificateIssuer|String|Issuer|
|certificateThumbprint|String|Thumbprint|
|certificateSerialNumber|String|Serial number|
|certificateKeyLength|Int32|Key length|
|certificateEnhancedKeyUsage|String|Extended key usage|
|certificateValidityPeriod|Int32|Validity period|
|certificateSubjectNameFormatString|String|Subject name format string for custom subject name formats|
|certificateSubjectAlternativeNameFormatString|String|Subject alternative name format string for custom formats|
|certificateIssuanceDateTime|DateTimeOffset|Issuance date|
|certificateErrorCode|Int32|Error code|



## Response
If successful, this method returns a `201 Created` response code and a [managedDeviceCertificateState](../resources/manageddevicecertificatestate.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_manageddevicecertificatestate_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates
Content-type: application/json
Content-length: 1449

{
  "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
  "devicePlatform": "String",
  "certificateKeyUsage": "String",
  "certificateValidityPeriodUnits": "String",
  "certificateIssuanceState": "String",
  "certificateKeyStorageProvider": "String",
  "certificateSubjectNameFormat": "String",
  "certificateSubjectAlternativeNameFormat": "String",
  "certificateRevokeStatus": "String",
  "certificateProfileDisplayName": "Certificate Profile Display Name value",
  "deviceDisplayName": "Device Display Name value",
  "userDisplayName": "User Display Name value",
  "certificateExpirationDateTime": "2016-12-31T23:57:57.5583647+03:00",
  "certificateLastIssuanceStateChangedDateTime": "2017-01-01T00:03:32.3703864+03:00",
  "lastCertificateStateChangeDateTime": "2016-12-31T23:58:49.2604406+03:00",
  "certificateIssuer": "Certificate Issuer value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateKeyLength": 4,
  "certificateEnhancedKeyUsage": "Certificate Enhanced Key Usage value",
  "certificateValidityPeriod": 9,
  "certificateSubjectNameFormatString": "Certificate Subject Name Format String value",
  "certificateSubjectAlternativeNameFormatString": "Certificate Subject Alternative Name Format String value",
  "certificateIssuanceDateTime": "2016-12-31T23:58:16.9914339+03:00",
  "certificateErrorCode": 4
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.manageddevicecertificatestate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1498

{
  "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
  "id": "d20e886a-886a-d20e-6a88-0ed26a880ed2",
  "devicePlatform": "String",
  "certificateKeyUsage": "String",
  "certificateValidityPeriodUnits": "String",
  "certificateIssuanceState": "String",
  "certificateKeyStorageProvider": "String",
  "certificateSubjectNameFormat": "String",
  "certificateSubjectAlternativeNameFormat": "String",
  "certificateRevokeStatus": "String",
  "certificateProfileDisplayName": "Certificate Profile Display Name value",
  "deviceDisplayName": "Device Display Name value",
  "userDisplayName": "User Display Name value",
  "certificateExpirationDateTime": "2016-12-31T23:57:57.5583647+03:00",
  "certificateLastIssuanceStateChangedDateTime": "2017-01-01T00:03:32.3703864+03:00",
  "lastCertificateStateChangeDateTime": "2016-12-31T23:58:49.2604406+03:00",
  "certificateIssuer": "Certificate Issuer value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateKeyLength": 4,
  "certificateEnhancedKeyUsage": "Certificate Enhanced Key Usage value",
  "certificateValidityPeriod": 9,
  "certificateSubjectNameFormatString": "Certificate Subject Name Format String value",
  "certificateSubjectAlternativeNameFormatString": "Certificate Subject Alternative Name Format String value",
  "certificateIssuanceDateTime": "2016-12-31T23:58:16.9914339+03:00",
  "certificateErrorCode": 4
}
```

