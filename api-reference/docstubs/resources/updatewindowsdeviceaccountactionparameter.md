---
title: "updateWindowsDeviceAccountActionParameter resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# updateWindowsDeviceAccountActionParameter resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|calendarSyncEnabled|Boolean|**TODO: Add Description**|
|deviceAccount|[windowsDeviceAccount](../resources/windowsdeviceaccount.md)|**TODO: Add Description**|
|deviceAccountEmail|String|**TODO: Add Description**|
|exchangeServer|String|**TODO: Add Description**|
|passwordRotationEnabled|Boolean|**TODO: Add Description**|
|sessionInitiationProtocalAddress|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.updateWindowsDeviceAccountActionParameter",
  "deviceAccount": {
    "@odata.type": "microsoft.graph.windowsDeviceAccount",
    "password": "String"
  },
  "passwordRotationEnabled": true,
  "calendarSyncEnabled": true,
  "deviceAccountEmail": "String",
  "exchangeServer": "String",
  "sessionInitiationProtocalAddress": "String"
}
```

