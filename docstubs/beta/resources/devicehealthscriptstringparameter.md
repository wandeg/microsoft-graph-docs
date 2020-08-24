---
title: "deviceHealthScriptStringParameter resource type"
description: "Properties of the  String script parameter."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# deviceHealthScriptStringParameter resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Properties of the  String script parameter.

## Properties

| Property                         | Type    | Description                                  |
| :------------------------------- | :------ | :------------------------------------------- |
| applyDefaultValueWhenNotAssigned | Boolean | Whether Apply DefaultValue When Not Assigned |
| defaultValue                     | String  | The default value of string param            |
| description                      | String  | The description of the param                 |
| isRequired                       | Boolean | Whether the param is required                |
| name                             | String  | The name of the param                        |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptStringParameter",
  "applyDefaultValueWhenNotAssigned": "Boolean",
  "defaultValue": "String",
  "description": "String",
  "isRequired": "Boolean",
  "name": "String"
}
```