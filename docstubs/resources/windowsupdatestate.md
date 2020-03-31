---
title: "windowsUpdateState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsUpdateState resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsUpdateState](../api/windowsupdatestate-get.md)|[windowsUpdateState](../resources/windowsupdatestate.md)|Read properties and relationships of the [windowsUpdateState](../resources/windowsupdatestate.md) object.|
|[Update windowsUpdateState](../api/windowsupdatestate-update.md)|[windowsUpdateState](../resources/windowsupdatestate.md)|Update the properties of a [windowsUpdateState](../resources/windowsupdatestate.md) object.|
|[List deviceUpdateStates](../api/windowsfeatureupdateprofile-list-deviceupdatestates.md)|[windowsUpdateState](../resources/windowsupdatestate.md) collection|Get the windowsUpdateStates from the deviceUpdateStates navigation property.|
|[Add deviceUpdateStates](../api/windowsfeatureupdateprofile-post-deviceupdatestates.md)|[windowsUpdateState](../resources/windowsupdatestate.md)|Add deviceUpdateStates by posting to the deviceUpdateStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceDisplayName|String||
|deviceId|String||
|featureUpdateVersion|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastScanDateTime|DateTimeOffset||
|lastSyncDateTime|DateTimeOffset||
|qualityUpdateVersion|String||
|status|Enumeration| Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.|
|userId|String||
|userPrincipalName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdateState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "id": "String (identifier)",
  "deviceId": "String",
  "userId": "String",
  "deviceDisplayName": "String",
  "userPrincipalName": "String",
  "status": "String",
  "qualityUpdateVersion": "String",
  "featureUpdateVersion": "String",
  "lastScanDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)"
}
```

