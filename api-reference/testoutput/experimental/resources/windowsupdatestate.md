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
|[List windowsUpdateStates](../api/windowsupdatestate-list.md)|[windowsUpdateState](../resources/windowsupdatestate.md) collection|List properties and relationships of the [windowsUpdateState](../resources/windowsupdatestate.md) objects.|
|[Get windowsUpdateState](../api/windowsupdatestate-get.md)|[windowsUpdateState](../resources/windowsupdatestate.md)|Read properties and relationships of the [windowsUpdateState](../resources/windowsupdatestate.md) object.|
|[Create windowsUpdateState](../api/windowsupdatestate-create.md)|[windowsUpdateState](../resources/windowsupdatestate.md)|Create a new [windowsUpdateState](../resources/windowsupdatestate.md) object.|
|[Delete windowsUpdateState](../api/windowsupdatestate-delete.md)|None|Deletes a [windowsUpdateState](../resources/windowsupdatestate.md).|
|[Update windowsUpdateState](../api/windowsupdatestate-update.md)|[windowsUpdateState](../resources/windowsupdatestate.md)|Update the properties of a [windowsUpdateState](../resources/windowsupdatestate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceDisplayName|String|Device display name.|
|deviceId|String|The id of the device.|
|featureUpdateVersion|String|The current feature update version of the device.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastScanDateTime|DateTimeOffset|The date time that the Windows Update Agent did a successful scan.|
|lastSyncDateTime|DateTimeOffset|Last date time that the device sync with with Microsoft Intune.|
|qualityUpdateVersion|String|The Quality Update Version of the device.|
|status|Enumeration|Windows udpate status. Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.|
|userId|String|The id of the user.|
|userPrincipalName|String|User principal name.|

## Relationships
None

## JSON Representation
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

