---
title: "Update userPFXCertificate"
description: "Update the properties of a userPFXCertificate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update userPFXCertificate

Namespace: microsoft.graph

Update the properties of a [userPFXCertificate](../resources/userpfxcertificate.md) object.

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
PATCH /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [userPFXCertificate](../resources/userpfxcertificate.md) object.

The following table shows the properties that are required when you create the [userPFXCertificate](../resources/userpfxcertificate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|thumbprint|String||
|intendedPurpose|Enumeration| Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.|
|userPrincipalName|String||
|startDateTime|DateTimeOffset||
|expirationDateTime|DateTimeOffset||
|providerName|String||
|keyName|String||
|paddingScheme|Enumeration| Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.|
|encryptedPfxBlob|Binary||
|encryptedPfxPassword|String||
|createdDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [userPFXCertificate](../resources/userpfxcertificate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_userpfxcertificate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates/{userPFXCertificateId}
Content-type: application/json
Content-length: 515

{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "thumbprint": "Thumbprint value",
  "intendedPurpose": "String",
  "userPrincipalName": "User Principal Name value",
  "startDateTime": "2017-01-01T00:03:15.8315541+03:00",
  "expirationDateTime": "2017-01-01T00:00:46.7802483+03:00",
  "providerName": "Provider Name value",
  "keyName": "Key Name value",
  "paddingScheme": "String",
  "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
  "encryptedPfxPassword": "Encrypted Pfx Password value"
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
Content-Length: 687

{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "id": "0d7c586c-586c-0d7c-6c58-7c0d6c587c0d",
  "thumbprint": "Thumbprint value",
  "intendedPurpose": "String",
  "userPrincipalName": "User Principal Name value",
  "startDateTime": "2017-01-01T00:03:15.8315541+03:00",
  "expirationDateTime": "2017-01-01T00:00:46.7802483+03:00",
  "providerName": "Provider Name value",
  "keyName": "Key Name value",
  "paddingScheme": "String",
  "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "createdDateTime": "2017-01-01T00:01:00.9969079+03:00",
  "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00"
}
```

