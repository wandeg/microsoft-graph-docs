---
title: "userPFXCertificate resource type"
description: "Entity that encapsulates all information required for a user's PFX certificates."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# userPFXCertificate resource type

Entity that encapsulates all information required for a user's PFX certificates.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userPFXCertificate](../api/userpfxcertificate-get.md)|[userPFXCertificate](../resources/userPFXCertificate.md)|Read properties and relationships of the [userPFXCertificate](../resources/userpfxcertificate.md) object.|
|[Delete userPFXCertificate](../api/userpfxcertificate-delete.md)|None|Deletes a [userPFXCertificate](../resources/userpfxcertificate.md).|
|[Update userPFXCertificate](../api/userpfxcertificate-update.md)|[userPFXCertificate](../resources/userPFXCertificate.md)|Update the properties of a [userPFXCertificate](../resources/userpfxcertificate.md) object.|
|[List userPfxCertificates](../api/intune-devices-devicemanagement-list-userpfxcertificates.md)|[userPFXCertificate](../resources/userPFXCertificate.md) collection|Get the userPFXCertificates from the userPfxCertificates navigation property.|
|[Add userPfxCertificates](../api/intune-devices-devicemanagement-post-userpfxcertificates.md)|[userPFXCertificate](../resources/userPFXCertificate.md)|Add userPfxCertificates by posting to the userPfxCertificates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Date/time when this PFX certificate was imported.|
|encryptedPfxBlob|Binary|Encrypted PFX blob.|
|encryptedPfxPassword|String|Encrypted PFX password.|
|expirationDateTime|DateTimeOffset|Certificate's validity expiration date/time.|
|id|String| Inherited from [entity](../resources/entity.md)|
|intendedPurpose|Enumeration|Certificate's intended purpose from the point-of-view of deployment. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.|
|keyName|String|Name of the key (within the provider) used to encrypt the blob.|
|lastModifiedDateTime|DateTimeOffset|Date/time when this PFX certificate was last modified.|
|paddingScheme|Enumeration|Padding scheme used by the provider during encryption/decryption. Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.|
|providerName|String|Crypto provider used to encrypt this blob.|
|startDateTime|DateTimeOffset|Certificate's validity start date/time.|
|thumbprint|String|SHA-1 thumbprint of the PFX certificate.|
|userPrincipalName|String|User Principal Name of the PFX certificate.|

## Relationships
None

## JSON Representation
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

