---
title: "hybridAgentUpdaterConfiguration resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# hybridAgentUpdaterConfiguration resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowUpdateConfigurationOverride|Boolean|**TODO: Add Description**|
|deferUpdateDateTime|DateTimeOffset|**TODO: Add Description**|
|updateWindow|[updateWindow](../resources/updatewindow.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.updateWindow"
  },
  "allowUpdateConfigurationOverride": "Boolean"
}
```

