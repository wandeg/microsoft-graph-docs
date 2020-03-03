---
title: "Get userPFXCertificate"
description: "Read properties and relationships of the userPFXCertificate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get userPFXCertificate

Namespace: microsoft.graph

Read properties and relationships of the [userPFXCertificate](../resources/userpfxcertificate.md) object.

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
GET /deviceManagement/userPfxCertificates/{userPFXCertificateId}
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
If successful, this method returns a `200 OK` response code and [userPFXCertificate](../resources/userpfxcertificate.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_userpfxcertificate"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userPFXCertificate"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 733

{
  "value": {
    "@odata.type": "#microsoft.graph.userPFXCertificate",
    "id": "56632ff6-2ff6-5663-f62f-6356f62f6356",
    "thumbprint": "Thumbprint value",
    "intendedPurpose": "String",
    "userPrincipalName": "User Principal Name value",
    "startDateTime": "2016-12-31T23:59:24.7548426+03:00",
    "expirationDateTime": "2016-12-31T23:59:56.1430588+03:00",
    "providerName": "Provider Name value",
    "keyName": "Key Name value",
    "paddingScheme": "String",
    "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
    "encryptedPfxPassword": "Encrypted Pfx Password value",
    "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
    "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00"
  }
}
```

