---
title: "printer resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# printer resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get printer](../api/printer-get.md)|[printer](../resources/printer.md)|Read properties and relationships of the [printer](../resources/printer.md) object.|
|[Update printer](../api/printer-update.md)|[printer](../resources/printer.md)|Update the properties of a [printer](../resources/printer.md) object.|
|[resetDefaults](../api/printer-resetdefaults.md)|None||
|[getCapabilities](../api/printer-getcapabilities.md)|[printerCapabilities](../resources/printercapabilities.md)||
|[List allowedUsers](../api/printer-list-allowedusers.md)|[printUserIdentity](../resources/printuseridentity.md) collection|Get the printUserIdentities from the allowedUsers navigation property.|
|[Add allowedUsers](../api/printer-post-allowedusers.md)|[printUserIdentity](../resources/printuseridentity.md)|Add allowedUsers by posting to the allowedUsers collection.|
|[List allowedGroups](../api/printer-list-allowedgroups.md)|[printIdentity](../resources/printidentity.md) collection|Get the printIdentities from the allowedGroups navigation property.|
|[Add allowedGroups](../api/printer-post-allowedgroups.md)|[printIdentity](../resources/printidentity.md)|Add allowedGroups by posting to the allowedGroups collection.|
|[List jobs](../api/printer-list-jobs.md)|[printJob](../resources/printjob.md) collection|Get the printJobs from the jobs navigation property.|
|[Add jobs](../api/printer-post-jobs.md)|[printJob](../resources/printjob.md)|Add jobs by posting to the jobs collection.|
|[Get printerShare](../api/printershare-get.md)|[printerShare](../resources/printershare.md)|Read properties and relationships of the [printerShare](../resources/printershare.md) object.|
|[List connectors](../api/printer-list-connectors.md)|[printConnector](../resources/printconnector.md) collection|Get the printConnectors from the connectors navigation property.|
|[Create connectors](../api/printer-post-connectors.md)|[printConnector](../resources/printconnector.md)|Create connectors by posting to the connectors collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|acceptingJobs|Boolean||
|defaults|[printerDefaults](../resources/printerdefaults.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|isShared|Boolean||
|location|[printerLocation](../resources/printerlocation.md)||
|manufacturer|String||
|model|String||
|name|String||
|registeredDateTime|DateTimeOffset||
|status|[printerStatus](../resources/printerstatus.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|allowedGroups|[printIdentity](../resources/printidentity.md) collection||
|allowedUsers|[printUserIdentity](../resources/printuseridentity.md) collection||
|connectors|[printConnector](../resources/printconnector.md) collection||
|jobs|[printJob](../resources/printjob.md) collection||
|share|[printerShare](../resources/printershare.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printer",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printer",
  "id": "String (identifier)",
  "name": "String",
  "manufacturer": "String",
  "model": "String",
  "registeredDateTime": "String (timestamp)",
  "status": {
    "@odata.type": "microsoft.graph.printerStatus"
  },
  "isShared": true,
  "acceptingJobs": true,
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "defaults": {
    "@odata.type": "microsoft.graph.printerDefaults"
  }
}
```

