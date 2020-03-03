---
title: "List symantecCodeSigningCertificates"
description: "List properties and relationships of the symantecCodeSigningCertificate objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List symantecCodeSigningCertificates

Namespace: microsoft.graph

List properties and relationships of the [symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md) objects.

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
GET ** Collection URI for microsoft.graph.symantecCodeSigningCertificate not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_symanteccodesigningcertificate"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.symantecCodeSigningCertificate not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.symanteccodesigningcertificate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 542

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
      "id": "686e5b1c-5b1c-686e-1c5b-6e681c5b6e68",
      "content": "Y29udGVudA==",
      "status": "String",
      "password": "Password value",
      "subjectName": "Subject Name value",
      "subject": "Subject value",
      "issuerName": "Issuer Name value",
      "issuer": "Issuer value",
      "expirationDateTime": "2016-12-31T23:59:56.1430588+03:00",
      "uploadDateTime": "2017-01-01T00:02:13.8421427+03:00"
    }
  ]
}
```

