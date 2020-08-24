---
title: "deviceCategory resource type"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# deviceCategory resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## Methods

| Method                                                   | Return Type                                    | Description                                                   |
| :------------------------------------------------------- | :--------------------------------------------- | :------------------------------------------------------------ |
| [List deviceCategory](../api/devicecategory-list.md)     | [deviceCategory](deviceCategory.md) collection | List properties and relationships of a deviceCategory object. |
| [Create deviceCategory](../api/devicecategory-create.md) | [deviceCategory](deviceCategory.md)            | Create a new deviceCategory object.                           |
| [Get deviceCategory](../api/devicecategory-get.md)       | [deviceCategory](deviceCategory.md)            | Read properties and relationships of a deviceCategory object. |
| [Update deviceCategory](../api/devicecategory-update.md) | [deviceCategory](deviceCategory.md)            | Update the properties of a deviceCategory object.             |
| [Delete deviceCategory](../api/devicecategory-delete.md) |                                                | Delete a deviceCategory object.                               |

## Properties

| Property | Type   | Description                                                      |
| :------- | :----- | :--------------------------------------------------------------- |
| id       | String | Unique identifier for the device category. Read-only. Read-only. |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)"
}
```