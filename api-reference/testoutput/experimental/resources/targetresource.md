---
title: "targetResource resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# targetResource resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|groupType|Enumeration|. Possible values are: `unifiedGroups`, `azureAD`, `unknownFutureValue`.|
|id|String||
|modifiedProperties|[modifiedProperty](../resources/modifiedProperty.md) collection||
|type|String||
|userPrincipalName|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.targetResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetResource",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String",
  "userPrincipalName": "String",
  "groupType": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.modifiedProperty",
      "oldValue": "String",
      "newValue": "String"
    }
  ]
}
```

