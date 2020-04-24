---
title: "windowsUpdateState resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsUpdateState resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsUpdateState](../api/windowsupdatestate-get.md)|[windowsUpdateState](../resources/windowsupdatestate.md)|Read the properties and relationships of a [windowsUpdateState](../resources/windowsupdatestate.md) object.|
|[Update windowsUpdateState](../api/windowsupdatestate-update.md)|[windowsUpdateState](../resources/windowsupdatestate.md)|Update the properties of a [windowsUpdateState](../resources/windowsupdatestate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceDisplayName|String|Device display name.|
|deviceId|String|The id of the device.|
|featureUpdateVersion|String|The current feature update version of the device.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastScanDateTime|DateTimeOffset|The date time that the Windows Update Agent did a successful scan.|
|lastSyncDateTime|DateTimeOffset|Last date time that the device sync with with Microsoft Intune.|
|qualityUpdateVersion|String|The Quality Update Version of the device.|
|status|windowsUpdateStatus|Windows udpate status. Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.|
|userId|String|The id of the user.|
|userPrincipalName|String|User principal name.|

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

