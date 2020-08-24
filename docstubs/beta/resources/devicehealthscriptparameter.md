---
title: "deviceHealthScriptParameter resource type"
description: "Base properties of the script parameter."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# deviceHealthScriptParameter resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Base properties of the script parameter.

## Properties

| Property                         | Type    | Description                                  |
| :------------------------------- | :------ | :------------------------------------------- |
| applyDefaultValueWhenNotAssigned | Boolean | Whether Apply DefaultValue When Not Assigned |
| description                      | String  | The description of the param                 |
| isRequired                       | Boolean | Whether the param is required                |
| name                             | String  | The name of the param                        |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptParameter",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptParameter",
  "applyDefaultValueWhenNotAssigned": "Boolean",
  "description": "String",
  "isRequired": "Boolean",
  "name": "String"
}
```