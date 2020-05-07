---
title: "Update userPfxCertificates"
description: "Update the properties of a userPfxCertificates object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update userPfxCertificates

Namespace: microsoft.graph

Update the properties of a userPfxCertificates object.

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
PATCH /deviceManagement/userPfxCertificates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userPFXCertificate](../resources/userpfxcertificate.md) object.

The following table shows the properties that are required when you create the [userPFXCertificate](../resources/userpfxcertificate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|thumbprint|String|**TODO: Add Description**|
|intendedPurpose|userPfxIntendedPurpose|**TODO: Add Description**. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.|
|userPrincipalName|String|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|providerName|String|**TODO: Add Description**|
|keyName|String|**TODO: Add Description**|
|paddingScheme|userPfxPaddingScheme|**TODO: Add Description**. Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.|
|encryptedPfxBlob|Binary|**TODO: Add Description**|
|encryptedPfxPassword|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [userPFXCertificate](../resources/userpfxcertificate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_userpfxcertificates"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
Content-Type: application/json
Content-length: 395

{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "thumbprint": "String",
  "intendedPurpose": "String",
  "userPrincipalName": "String",
  "startDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "providerName": "String",
  "keyName": "String",
  "paddingScheme": "String",
  "encryptedPfxBlob": "Binary",
  "encryptedPfxPassword": "String"
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
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "id": "a6d4b911-b911-a6d4-11b9-d4a611b9d4a6",
  "thumbprint": "String",
  "intendedPurpose": "String",
  "userPrincipalName": "String",
  "startDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "providerName": "String",
  "keyName": "String",
  "paddingScheme": "String",
  "encryptedPfxBlob": "Binary",
  "encryptedPfxPassword": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

