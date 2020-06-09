---
title: "targetResource resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# targetResource resource type

Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|groupType|groupType|**TODO: Add Description**. Possible values are: `unifiedGroups`, `azureAD`, `unknownFutureValue`.|
|id|String|**TODO: Add Description**|
|modifiedProperties|[modifiedProperty](../resources/modifiedproperty.md) collection|**TODO: Add Description**|
|type|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
      "@odata.type": "microsoft.graph.modifiedProperty"
    }
  ]
}
```

