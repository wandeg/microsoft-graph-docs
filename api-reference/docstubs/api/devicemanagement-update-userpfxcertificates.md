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
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [userPFXCertificate](../resources/userpfxcertificate.md) object.

The following table shows the properties that are required when you create the [userPFXCertificate](../resources/userpfxcertificate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|thumbprint|String|SHA-1 thumbprint of the PFX certificate.|
|intendedPurpose|userPfxIntendedPurpose|Certificate's intended purpose from the point-of-view of deployment. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.|
|userPrincipalName|String|User Principal Name of the PFX certificate.|
|startDateTime|DateTimeOffset|Certificate's validity start date/time.|
|expirationDateTime|DateTimeOffset|Certificate's validity expiration date/time.|
|providerName|String|Crypto provider used to encrypt this blob.|
|keyName|String|Name of the key (within the provider) used to encrypt the blob.|
|paddingScheme|userPfxPaddingScheme|Padding scheme used by the provider during encryption/decryption. Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.|
|encryptedPfxBlob|Binary|Encrypted PFX blob.|
|encryptedPfxPassword|String|Encrypted PFX password.|
|createdDateTime|DateTimeOffset|Date/time when this PFX certificate was imported.|
|lastModifiedDateTime|DateTimeOffset|Date/time when this PFX certificate was last modified.|



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
Content-length: 514

{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "thumbprint": "Thumbprint value",
  "intendedPurpose": "String",
  "userPrincipalName": "User Principal Name value",
  "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "providerName": "Provider Name value",
  "keyName": "Key Name value",
  "paddingScheme": "String",
  "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
  "encryptedPfxPassword": "Encrypted Pfx Password value"
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
  "id": "d48f33f1-33f1-d48f-f133-8fd4f1338fd4",
  "thumbprint": "Thumbprint value",
  "intendedPurpose": "String",
  "userPrincipalName": "User Principal Name value",
  "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "providerName": "Provider Name value",
  "keyName": "Key Name value",
  "paddingScheme": "String",
  "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
}
```

