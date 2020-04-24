---
title: "userPFXCertificate resource type"
description: "Entity that encapsulates all information required for a user's PFX certificates."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userPFXCertificate resource type


Namespace: microsoft.graph

Entity that encapsulates all information required for a user's PFX certificates.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userPFXCertificate](../api/userpfxcertificate-get.md)|[userPFXCertificate](../resources/userpfxcertificate.md)|Read the properties and relationships of a [userPFXCertificate](../resources/userpfxcertificate.md) object.|
|[Update userPFXCertificate](../api/userpfxcertificate-update.md)|[userPFXCertificate](../resources/userpfxcertificate.md)|Update the properties of a [userPFXCertificate](../resources/userpfxcertificate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Date/time when this PFX certificate was imported.|
|encryptedPfxBlob|Binary|Encrypted PFX blob.|
|encryptedPfxPassword|String|Encrypted PFX password.|
|expirationDateTime|DateTimeOffset|Certificate's validity expiration date/time.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|intendedPurpose|userPfxIntendedPurpose|Certificate's intended purpose from the point-of-view of deployment. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.|
|keyName|String|Name of the key (within the provider) used to encrypt the blob.|
|lastModifiedDateTime|DateTimeOffset|Date/time when this PFX certificate was last modified.|
|paddingScheme|userPfxPaddingScheme|Padding scheme used by the provider during encryption/decryption. Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.|
|providerName|String|Crypto provider used to encrypt this blob.|
|startDateTime|DateTimeOffset|Certificate's validity start date/time.|
|thumbprint|String|SHA-1 thumbprint of the PFX certificate.|
|userPrincipalName|String|User Principal Name of the PFX certificate.|

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

