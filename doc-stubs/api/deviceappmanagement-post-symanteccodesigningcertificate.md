---
title: "Create symantecCodeSigningCertificate"
description: "Create a new symantecCodeSigningCertificate object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create symantecCodeSigningCertificate

Namespace: microsoft.graph

Create a new symantecCodeSigningCertificate object.

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
POST /deviceAppManagement/symantecCodeSigningCertificate
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md) object.

The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|content|Binary|**TODO: Add Description**|
|status|certificateStatus|**TODO: Add Description**. Possible values are: `notProvisioned`, `provisioned`.|
|password|String|**TODO: Add Description**|
|subjectName|String|**TODO: Add Description**|
|subject|String|**TODO: Add Description**|
|issuerName|String|**TODO: Add Description**|
|issuer|String|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|uploadDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_symanteccodesigningcertificate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/symantecCodeSigningCertificate
Content-Type: application/json
Content-length: 336

{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "content": "Binary",
  "status": "String",
  "password": "String",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.symanteccodesigningcertificate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "eba3bdb0-bdb0-eba3-b0bd-a3ebb0bda3eb",
  "content": "Binary",
  "status": "String",
  "password": "String",
  "subjectName": "String",
  "subject": "String",
  "issuerName": "String",
  "issuer": "String",
  "expirationDateTime": "String (timestamp)",
  "uploadDateTime": "String (timestamp)"
}
```

