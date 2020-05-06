---
title: "deviceManagement resource type"
description: "Singleton that acts as container for a collection of UserPFXCertificate entities."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagement resource type


Namespace: microsoft.graph

Singleton that acts as container for a collection of UserPFXCertificate entities.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[Get deviceManagement](../api/intune-devicemanagement-get.md)|[deviceManagement](../resources/intune-devicemanagement.md)|Read the properties and relationships of a [deviceManagement](../resources/intune-devicemanagement.md) object.|
|[Update deviceManagement](../api/intune-devicemanagement-update.md)|[deviceManagement](../resources/intune-devicemanagement.md)|Update the properties of a [deviceManagement](../resources/intune-devicemanagement.md) object.|
|[List userPfxCertificates](../api/intune-devicemanagement-list-userpfxcertificates.md)|[userPFXCertificate](../resources/intune-userpfxcertificate.md) collection|Get the userPFXCertificates from the userPfxCertificates navigation property.|
|[Create userPfxCertificates](../api/intune-devicemanagement-post-userpfxcertificates.md)|[userPFXCertificate](../resources/intune-userpfxcertificate.md)|Create a new userPfxCertificates object.|
|[Delete userPfxCertificates](../api/intune-devicemanagement-delete-userpfxcertificates.md)|None|Delete a [userPFXCertificate](../resources/intune-userpfxcertificate.md) object.|
|[Update userPfxCertificates](../api/intune-devicemanagement-update-userpfxcertificates.md)|[userPFXCertificate](../resources/intune-userpfxcertificate.md)|Update the properties of a userPfxCertificates object.|
|[Get userPFXCertificate](../api/intune-userpfxcertificate-get.md)|[userPFXCertificate](../resources/intune-userpfxcertificate.md)|Read the properties and relationships of a [userPFXCertificate](../resources/intune-userpfxcertificate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|userPfxCertificates|[userPFXCertificate](../resources/intune-userpfxcertificate.md) collection|Collection of PFX certificates associated with a user.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.management.services.api.deviceManagement",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.deviceManagement",
  "id": "String (identifier)"
}
```

