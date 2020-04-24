---
title: "printerShare resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# printerShare resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get printerShare](../api/printershare-get.md)|[printerShare](../resources/printershare.md)|Read the properties and relationships of a [printerShare](../resources/printershare.md) object.|
|[Update printerShare](../api/printershare-update.md)|[printerShare](../resources/printershare.md)|Update the properties of a [printerShare](../resources/printershare.md) object.|
|[List printer](../api/printershare-list-printer.md)|[printer](../resources/printer.md) collection|Get the printers from the printer navigation property.|
|[Add printer](../api/printershare-post-printer.md)|[printer](../resources/printer.md)|Add printer by posting to the printer collection.|
|[Remove printer](../api/printershare-delete-printer.md)|None|Remove a [printer](../resources/printer.md) object.|
|[List allowedUsers](../api/printershare-list-allowedusers.md)|[printUserIdentity](../resources/printuseridentity.md) collection|Get the printUserIdentities from the allowedUsers navigation property.|
|[Create allowedUsers](../api/printershare-post-allowedusers.md)|[printUserIdentity](../resources/printuseridentity.md)|Create a new allowedUsers object.|
|[Delete allowedUsers](../api/printershare-delete-allowedusers.md)|None|Delete an [printUserIdentity](../resources/printuseridentity.md) object.|
|[Update allowedUsers](../api/printershare-update-allowedusers.md)|[printUserIdentity](../resources/printuseridentity.md)|Update the properties of an allowedUsers object.|
|[Get printUserIdentity](../api/printuseridentity-get.md)|[printUserIdentity](../resources/printuseridentity.md)|Read the properties and relationships of a [printUserIdentity](../resources/printuseridentity.md) object.|
|[List allowedGroups](../api/printershare-list-allowedgroups.md)|[printIdentity](../resources/printidentity.md) collection|Get the printIdentities from the allowedGroups navigation property.|
|[Create allowedGroups](../api/printershare-post-allowedgroups.md)|[printIdentity](../resources/printidentity.md)|Create a new allowedGroups object.|
|[Delete allowedGroups](../api/printershare-delete-allowedgroups.md)|None|Delete an [printIdentity](../resources/printidentity.md) object.|
|[Update allowedGroups](../api/printershare-update-allowedgroups.md)|[printIdentity](../resources/printidentity.md)|Update the properties of an allowedGroups object.|
|[Get printIdentity](../api/printidentity-get.md)|[printIdentity](../resources/printidentity.md)|Read the properties and relationships of a [printIdentity](../resources/printidentity.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|allowedGroups|[printIdentity](../resources/printidentity.md) collection|**TODO: Add Description**|
|allowedUsers|[printUserIdentity](../resources/printuseridentity.md) collection|**TODO: Add Description**|
|printer|[printer](../resources/printer.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printerShare",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerShare",
  "id": "String (identifier)",
  "name": "String",
  "createdDateTime": "String (timestamp)"
}
```

