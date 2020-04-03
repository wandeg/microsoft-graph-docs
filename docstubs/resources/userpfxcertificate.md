---
title: "userPFXCertificate resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userPFXCertificate resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userPFXCertificate](../api/userpfxcertificate-get.md)|[userPFXCertificate](../resources/userpfxcertificate.md)|Read properties and relationships of the [userPFXCertificate](../resources/userpfxcertificate.md) object.|
|[Update userPFXCertificate](../api/userpfxcertificate-update.md)|[userPFXCertificate](../resources/userpfxcertificate.md)|Update the properties of a [userPFXCertificate](../resources/userpfxcertificate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|encryptedPfxBlob|Binary||
|encryptedPfxPassword|String||
|expirationDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|intendedPurpose|Enumeration| Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.|
|keyName|String||
|lastModifiedDateTime|DateTimeOffset||
|paddingScheme|Enumeration| Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.|
|providerName|String||
|startDateTime|DateTimeOffset||
|thumbprint|String||
|userPrincipalName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userPFXCertificate",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "id": "String (identifier)",
  "thumbprint": "String",
  "intendedPurpose": "String",
  "userPrincipalName": "String",
  "startDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "providerName": "String",
  "keyName": "String",
  "paddingScheme": "String",
  "encryptedPfxBlob": "binary",
  "encryptedPfxPassword": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

