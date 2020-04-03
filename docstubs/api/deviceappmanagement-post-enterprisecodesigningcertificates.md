---
title: "Add enterpriseCodeSigningCertificates"
description: "Add enterpriseCodeSigningCertificates by posting to the enterpriseCodeSigningCertificates collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add enterpriseCodeSigningCertificates

Namespace: microsoft.graph

Add enterpriseCodeSigningCertificates by posting to the enterpriseCodeSigningCertificates collection.

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
POST /deviceAppManagement/enterpriseCodeSigningCertificates/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [enterpriseCodeSigningCertificate](../resources/enterprisecodesigningcertificate.md) object.

The following table shows the properties that are required when you create the [enterpriseCodeSigningCertificate](../resources/enterprisecodesigningcertificate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|content|Binary||
|status|Enumeration| Possible values are: `notProvisioned`, `provisioned`.|
|subjectName|String||
|subject|String||
|issuerName|String||
|issuer|String||
|expirationDateTime|DateTimeOffset||
|uploadDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [enterpriseCodeSigningCertificate](../resources/enterprisecodesigningcertificate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_enterprisecodesigningcertificate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates
Content-type: application/json
Content-length: 385

{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "content": "Y29udGVudA==",
  "status": "String",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:47.0232285+00:00",
  "uploadDateTime": "2016-12-31T23:56:37.4295814+00:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.enterprisecodesigningcertificate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 434

{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "id": "ccacec3e-ec3e-ccac-3eec-accc3eecaccc",
  "content": "Y29udGVudA==",
  "status": "String",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:47.0232285+00:00",
  "uploadDateTime": "2016-12-31T23:56:37.4295814+00:00"
}
```

