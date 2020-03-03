---
title: "Get managedDeviceCertificateState"
description: "Read properties and relationships of the managedDeviceCertificateState object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get managedDeviceCertificateState

Read properties and relationships of the [managedDeviceCertificateState](../resources/manageddevicecertificatestate.md) object.

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
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [managedDeviceCertificateState](../resources/manageddevicecertificatestate.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_manageddevicecertificatestate"
}
-->
``` http

```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedDeviceCertificateState"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1569

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
    "id": "11e07268-7268-11e0-6872-e0116872e011",
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
    "certificateExpirationDateTime": "2016-12-31T23:59:01.3955648+03:00",
    "certificateLastIssuanceStateChangedDateTime": "2016-12-31T23:59:52.1845752+03:00",
    "lastCertificateStateChangeDateTime": "2016-12-31T23:56:46.3178631+03:00",
    "certificateIssuer": "Certificate Issuer value",
    "certificateThumbprint": "Certificate Thumbprint value",
    "certificateSerialNumber": "Certificate Serial Number value",
    "certificateKeyLength": 4,
    "certificateEnhancedKeyUsage": "Certificate Enhanced Key Usage value",
    "certificateValidityPeriod": 9,
    "certificateSubjectNameFormatString": "Certificate Subject Name Format String value",
    "certificateSubjectAlternativeNameFormatString": "Certificate Subject Alternative Name Format String value",
    "certificateIssuanceDateTime": "2017-01-01T00:00:11.2022147+03:00",
    "certificateErrorCode": 4
  }
}
```

