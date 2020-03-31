---
title: "hybridAgentUpdaterConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# hybridAgentUpdaterConfiguration resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowUpdateConfigurationOverride|Boolean||
|deferUpdateDateTime|DateTimeOffset||
|updateWindow|[updateWindow](../resources/updatewindow.md)||

## Relationships
None

## JSON representation
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

