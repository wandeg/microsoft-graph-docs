---
title: "hybridAgentUpdaterConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# hybridAgentUpdaterConfiguration resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowUpdateConfigurationOverride|Boolean||
|deferUpdateDateTime|DateTimeOffset||
|updateWindow|[updateWindow](../resources/updateWindow.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hybridAgentUpdaterConfiguration",
  "deferUpdateDateTime": "String (timestamp)",
  "updateWindow": {
    "@odata.type": "microsoft.graph.updateWindow",
    "updateWindowStartTime": "String (time of day)",
    "updateWindowEndTime": "String (time of day)"
  },
  "allowUpdateConfigurationOverride": true
}
```

