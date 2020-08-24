---
title: "deviceHealthScriptBooleanParameter resource type"
description: "Properties of the  Booolean script parameter."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# deviceHealthScriptBooleanParameter resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Properties of the  Booolean script parameter.

## Properties

| Property                         | Type    | Description                                  |
| :------------------------------- | :------ | :------------------------------------------- |
| applyDefaultValueWhenNotAssigned | Boolean | Whether Apply DefaultValue When Not Assigned |
| defaultValue                     | Boolean | The default value of boolean param           |
| description                      | String  | The description of the param                 |
| isRequired                       | Boolean | Whether the param is required                |
| name                             | String  | The name of the param                        |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptBooleanParameter",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptBooleanParameter",
  "applyDefaultValueWhenNotAssigned": "Boolean",
  "defaultValue": "Boolean",
  "description": "String",
  "isRequired": "Boolean",
  "name": "String"
}
```