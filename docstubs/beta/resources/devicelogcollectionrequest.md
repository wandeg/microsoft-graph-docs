---
title: "deviceLogCollectionRequest resource type"
description: "Windows Log Collection request entity."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# deviceLogCollectionRequest resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Windows Log Collection request entity.

## Properties

| Property     | Type   | Description                                                |
| :----------- | :----- | :--------------------------------------------------------- |
| id           | String | The unique identifier                                      |
| templateType | String | The template type that is sent with the collection request |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceLogCollectionRequest",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceLogCollectionRequest",
  "id": "String",
  "templateType": "predefined"
}
```