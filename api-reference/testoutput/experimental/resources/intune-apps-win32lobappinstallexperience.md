---
title: "win32LobAppInstallExperience resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# win32LobAppInstallExperience resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceRestartBehavior|Enumeration|Device restart behavior. Possible values are: `basedOnReturnCode`, `allow`, `suppress`, `force`.|
|runAsAccount|Enumeration|Indicates the type of execution context the app runs in. Possible values are: `system`, `user`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "runAsAccount": "String",
  "deviceRestartBehavior": "String"
}
```

