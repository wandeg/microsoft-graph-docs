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


Inherits from [printerBase](../resources/printerbase.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List jobs](../api/printershare-list-jobs.md)|[printJob](../resources/printjob.md) collection|Get the printJobs from the jobs navigation property.|
|[Create jobs](../api/printershare-post-jobs.md)|[printJob](../resources/printjob.md)|Create a new jobs object.|
|[Delete jobs](../api/printershare-delete-jobs.md)|None|Delete a [printJob](../resources/printjob.md) object.|
|[Update jobs](../api/printershare-update-jobs.md)|[printJob](../resources/printjob.md)|Update the properties of a jobs object.|
|[Get printJob](../api/printjob-get.md)|[printJob](../resources/printjob.md)|Read the properties and relationships of a [printJob](../resources/printjob.md) object.|
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
|[List share](../api/printer-list-share.md)|[printerShare](../resources/printershare.md) collection|Get the printerShares from the share navigation property.|
|[Add share](../api/printer-post-share.md)|[printerShare](../resources/printershare.md)|Add share by posting to the share collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|capabilities|[printerCapabilities](../resources/printercapabilities.md)|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|defaults|[printerDefaults](../resources/printerdefaults.md)|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isAcceptingJobs|Boolean|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md)|
|location|[printerLocation](../resources/printerlocation.md)|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md)|
|manufacturer|String|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md)|
|model|String|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md)|
|name|String|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md)|
|status|[printerStatus](../resources/printerstatus.md)|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|allowedGroups|[printIdentity](../resources/printidentity.md) collection|**TODO: Add Description**|
|allowedUsers|[printUserIdentity](../resources/printuseridentity.md) collection|**TODO: Add Description**|
|jobs|[printJob](../resources/printjob.md) collection|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md)|
|printer|[printer](../resources/printer.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printerShare",
  "baseType": "microsoft.graph.printerBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerShare",
  "id": "String (identifier)",
  "name": "String",
  "manufacturer": "String",
  "model": "String",
  "isAcceptingJobs": "Boolean",
  "defaults": {
    "@odata.type": "microsoft.graph.printerDefaults"
  },
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "capabilities": {
    "@odata.type": "microsoft.graph.printerCapabilities"
  },
  "status": {
    "@odata.type": "microsoft.graph.printerStatus"
  },
  "createdDateTime": "String (timestamp)"
}
```

