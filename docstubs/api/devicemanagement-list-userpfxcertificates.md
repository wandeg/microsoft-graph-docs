---
title: "List userPfxCertificates"
description: "Get the userPFXCertificates from the userPfxCertificates navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List userPfxCertificates

Namespace: microsoft.graph

Get the userPFXCertificates from the userPfxCertificates navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userPfxCertificates
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [userPFXCertificate](../resources/userpfxcertificate.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_userpfxcertificate"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.userpfxcertificate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 775

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userPFXCertificate",
      "id": "f7aed8d2-d8d2-f7ae-d2d8-aef7d2d8aef7",
      "thumbprint": "Thumbprint value",
      "intendedPurpose": "String",
      "userPrincipalName": "User Principal Name value",
      "startDateTime": "2017-01-01T00:03:09.5259332+03:00",
      "expirationDateTime": "2016-12-31T23:56:49.0349895+03:00",
      "providerName": "Provider Name value",
      "keyName": "Key Name value",
      "paddingScheme": "String",
      "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
      "encryptedPfxPassword": "Encrypted Pfx Password value",
      "createdDateTime": "2016-12-31T23:58:10.4520456+03:00",
      "lastModifiedDateTime": "2017-01-01T00:02:23.471109+03:00"
    }
  ]
}
```

