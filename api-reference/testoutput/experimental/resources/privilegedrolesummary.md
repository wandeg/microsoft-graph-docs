---
title: "privilegedRoleSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# privilegedRoleSummary resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List privilegedRoleSummaries](../api/privilegedrolesummary-list.md)|[privilegedRoleSummary](../resources/privilegedRoleSummary.md) collection|List properties and relationships of the [privilegedRoleSummary](../resources/privilegedrolesummary.md) objects.|
|[Get privilegedRoleSummary](../api/privilegedrolesummary-get.md)|[privilegedRoleSummary](../resources/privilegedRoleSummary.md)|Read properties and relationships of the [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.|
|[Create privilegedRoleSummary](../api/privilegedrolesummary-create.md)|[privilegedRoleSummary](../resources/privilegedRoleSummary.md)|Create a new [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.|
|[Delete privilegedRoleSummary](../api/privilegedrolesummary-delete.md)|None|Deletes a [privilegedRoleSummary](../resources/privilegedrolesummary.md).|
|[Update privilegedRoleSummary](../api/privilegedrolesummary-update.md)|[privilegedRoleSummary](../resources/privilegedRoleSummary.md)|Update the properties of a [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|elevatedCount|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|managedCount|Int32||
|mfaEnabled|Boolean||
|status|Enumeration|. Possible values are: `ok`, `bad`.|
|usersCount|Int32||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.privilegedRoleSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.privilegedRoleSummary",
  "id": "String (identifier)",
  "status": "String",
  "usersCount": 1024,
  "managedCount": 1024,
  "elevatedCount": 1024,
  "mfaEnabled": true
}
```

