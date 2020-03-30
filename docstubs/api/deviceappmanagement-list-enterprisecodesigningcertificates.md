---
title: "List enterpriseCodeSigningCertificates"
description: "Get the enterpriseCodeSigningCertificates from the enterpriseCodeSigningCertificates navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List enterpriseCodeSigningCertificates

Namespace: microsoft.graph

Get the enterpriseCodeSigningCertificates from the enterpriseCodeSigningCertificates navigation property.

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
GET /deviceAppManagement/enterpriseCodeSigningCertificates
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
If successful, this method returns a `200 OK` response code and a collection of [enterpriseCodeSigningCertificate](../resources/enterprisecodesigningcertificate.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_enterprisecodesigningcertificate"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.enterprisecodesigningcertificate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 507

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
      "id": "d732b735-b735-d732-35b7-32d735b732d7",
      "content": "Y29udGVudA==",
      "status": "String",
      "subjectName": "Subject Name value",
      "subject": "Subject value",
      "issuerName": "Issuer Name value",
      "issuer": "Issuer value",
      "expirationDateTime": "2016-12-31T23:58:48.8634396+03:00",
      "uploadDateTime": "2016-12-31T23:58:51.3808857+03:00"
    }
  ]
}
```

