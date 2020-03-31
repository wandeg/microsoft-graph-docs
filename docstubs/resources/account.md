---
title: "account resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# account resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get account](../api/account-get.md)|[account](../resources/account.md)|Read properties and relationships of the [account](../resources/account.md) object.|
|[Update account](../api/account-update.md)|[account](../resources/account.md)|Update the properties of a [account](../resources/account.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|blocked|Boolean||
|category|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|number|String||
|subCategory|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.account",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.account",
  "id": "String (identifier)",
  "number": "String",
  "displayName": "String",
  "category": "String",
  "subCategory": "String",
  "blocked": true,
  "lastModifiedDateTime": "String (timestamp)"
}
```

