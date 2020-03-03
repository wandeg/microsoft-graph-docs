---
title: "updateWindowsDeviceAccountActionParameter resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# updateWindowsDeviceAccountActionParameter resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|calendarSyncEnabled|Boolean||
|deviceAccount|[windowsDeviceAccount](../resources/windowsDeviceAccount.md)||
|deviceAccountEmail|String||
|exchangeServer|String||
|passwordRotationEnabled|Boolean||
|sessionInitiationProtocalAddress|String||

## Relationships
None

## JSON Representation
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

