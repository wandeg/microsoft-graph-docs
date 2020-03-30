---
title: "Update symantecCodeSigningCertificate"
description: "Update the properties of a symantecCodeSigningCertificate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update symantecCodeSigningCertificate

Namespace: microsoft.graph

Update the properties of a [symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md) object.

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
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md) object.

The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|content|Binary||
|status|Enumeration| Possible values are: `notProvisioned`, `provisioned`.|
|password|String||
|subjectName|String||
|subject|String||
|issuerName|String||
|issuer|String||
|expirationDateTime|DateTimeOffset||
|uploadDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_symanteccodesigningcertificate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/symantecCodeSigningCertificate
Content-type: application/json
Content-length: 416

{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "content": "Y29udGVudA==",
  "status": "String",
  "password": "Password value",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:59:40.5485728+00:00",
  "uploadDateTime": "2017-01-01T00:00:18.1206183+00:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 465

{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "1d2a901e-901e-1d2a-1e90-2a1d1e902a1d",
  "content": "Y29udGVudA==",
  "status": "String",
  "password": "Password value",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:59:40.5485728+00:00",
  "uploadDateTime": "2017-01-01T00:00:18.1206183+00:00"
}
```

