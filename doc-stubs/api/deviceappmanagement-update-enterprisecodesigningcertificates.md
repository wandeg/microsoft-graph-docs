---
title: "Update enterpriseCodeSigningCertificates"
description: "Update the properties of an enterpriseCodeSigningCertificates object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update enterpriseCodeSigningCertificates

Namespace: microsoft.graph

Update the properties of an enterpriseCodeSigningCertificates object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/enterpriseCodeSigningCertificates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [enterpriseCodeSigningCertificate](../resources/enterprisecodesigningcertificate.md) object.

The following table shows the properties that are required when you create the [enterpriseCodeSigningCertificate](../resources/enterprisecodesigningcertificate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|content|Binary|**TODO: Add Description**|
|status|certificateStatus|**TODO: Add Description**. Possible values are: `notProvisioned`, `provisioned`.|
|subjectName|String|**TODO: Add Description**|
|subject|String|**TODO: Add Description**|
|issuerName|String|**TODO: Add Description**|
|issuer|String|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|uploadDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [enterpriseCodeSigningCertificate](../resources/enterprisecodesigningcertificate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_enterprisecodesigningcertificates"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates
Content-Type: application/json
Content-length: 313

{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "content": "Binary",
  "status": "String",
  "subjectName": "String",
  "subject": "String",
  "issuerName": "String",
  "issuer": "String",
  "expirationDateTime": "String (timestamp)",
  "uploadDateTime": "String (timestamp)"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "id": "9d4aeb7a-eb7a-9d4a-7aeb-4a9d7aeb4a9d",
  "content": "Binary",
  "status": "String",
  "subjectName": "String",
  "subject": "String",
  "issuerName": "String",
  "issuer": "String",
  "expirationDateTime": "String (timestamp)",
  "uploadDateTime": "String (timestamp)"
}
```

