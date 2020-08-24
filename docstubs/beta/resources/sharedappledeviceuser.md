---
title: "sharedAppleDeviceUser resource type"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# sharedAppleDeviceUser resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## Properties

| Property          | Type    | Description  |
| :---------------- | :------ | :----------- |
| dataQuota         | Int64   | Data quota   |
| dataToSync        | Boolean | Data to sync |
| dataUsed          | Int64   | Data quota   |
| userPrincipalName | String  | User name    |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.sharedAppleDeviceUser",
  "dataQuota": "Int64",
  "dataToSync": "Boolean",
  "dataUsed": "Int64",
  "userPrincipalName": "String"
}
```