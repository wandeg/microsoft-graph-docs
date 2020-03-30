---
title: "telecomExpenseManagementPartner resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# telecomExpenseManagementPartner resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get telecomExpenseManagementPartner](../api/telecomexpensemanagementpartner-get.md)|[telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md)|Read properties and relationships of the [telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) object.|
|[Update telecomExpenseManagementPartner](../api/telecomexpensemanagementpartner-update.md)|[telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md)|Update the properties of a [telecomExpenseManagementPartner](../resources/telecomexpensemanagementpartner.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appAuthorized|Boolean||
|displayName|String||
|enabled|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastConnectionDateTime|DateTimeOffset||
|url|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.telecomExpenseManagementPartner",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "String (identifier)",
  "displayName": "String",
  "url": "String",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "String (timestamp)"
}
```

