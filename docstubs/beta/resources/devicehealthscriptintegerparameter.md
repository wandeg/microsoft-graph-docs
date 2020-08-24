---
title: "deviceHealthScriptIntegerParameter resource type"
description: "Properties of the  Integer script parameter."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# deviceHealthScriptIntegerParameter resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Properties of the  Integer script parameter.

## Properties

| Property                         | Type    | Description                                                                |
| :------------------------------- | :------ | :------------------------------------------------------------------------- |
| applyDefaultValueWhenNotAssigned | Boolean | Whether Apply DefaultValue When Not Assigned                               |
| defaultValue                     | Int32   | The default value of Integer param. Valid values -2147483648 to 2147483647 |
| description                      | String  | The description of the param                                               |
| isRequired                       | Boolean | Whether the param is required                                              |
| name                             | String  | The name of the param                                                      |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptIntegerParameter",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptIntegerParameter",
  "applyDefaultValueWhenNotAssigned": "Boolean",
  "defaultValue": "Int32",
  "description": "String",
  "isRequired": "Boolean",
  "name": "String"
}
```