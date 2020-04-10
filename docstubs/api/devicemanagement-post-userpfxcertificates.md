---
title: "Add userPfxCertificates"
description: "Add userPfxCertificates by posting to the userPfxCertificates collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add userPfxCertificates

Namespace: microsoft.graph

Add userPfxCertificates by posting to the userPfxCertificates collection.

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
POST /deviceManagement/userPfxCertificates/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [userPFXCertificate](../resources/userpfxcertificate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_userpfxcertificate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
Content-type: application/json
Content-length: 515

{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "thumbprint": "Thumbprint value",
  "intendedPurpose": "String",
  "userPrincipalName": "User Principal Name value",
  "startDateTime": "2016-12-31T23:57:39.2677321+00:00",
  "expirationDateTime": "2016-12-31T23:56:24.5775752+00:00",
  "providerName": "Provider Name value",
  "keyName": "Key Name value",
  "paddingScheme": "String",
  "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
  "encryptedPfxPassword": "Encrypted Pfx Password value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userpfxcertificate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 687

{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "id": "6a1b33c4-33c4-6a1b-c433-1b6ac4331b6a",
  "thumbprint": "Thumbprint value",
  "intendedPurpose": "String",
  "userPrincipalName": "User Principal Name value",
  "startDateTime": "2016-12-31T23:57:39.2677321+00:00",
  "expirationDateTime": "2016-12-31T23:56:24.5775752+00:00",
  "providerName": "Provider Name value",
  "keyName": "Key Name value",
  "paddingScheme": "String",
  "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
  "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00"
}
```

