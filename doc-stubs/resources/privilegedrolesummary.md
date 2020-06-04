---
title: "privilegedRoleSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# privilegedRoleSummary resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List privilegedRoleSummaries](../api/privilegedrolesummary-list.md)|[privilegedRoleSummary](../resources/privilegedrolesummary.md) collection|Get a list of the [privilegedRoleSummary](../resources/privilegedrolesummary.md) objects and their properties.|
|[Create privilegedRoleSummary](../api/privilegedrolesummary-create.md)|[privilegedRoleSummary](../resources/privilegedrolesummary.md)|Create a new [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.|
|[Get privilegedRoleSummary](../api/privilegedrolesummary-get.md)|[privilegedRoleSummary](../resources/privilegedrolesummary.md)|Read the properties and relationships of a [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.|
|[Update privilegedRoleSummary](../api/privilegedrolesummary-update.md)|[privilegedRoleSummary](../resources/privilegedrolesummary.md)|Update the properties of a [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.|
|[Delete privilegedRoleSummary](../api/privilegedrolesummary-delete.md)|None|Deletes a [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|elevatedCount|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|managedCount|Int32|**TODO: Add Description**|
|mfaEnabled|Boolean|**TODO: Add Description**|
|status|roleSummaryStatus|**TODO: Add Description**. Possible values are: `ok`, `bad`.|
|usersCount|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "usersCount": "Integer",
  "managedCount": "Integer",
  "elevatedCount": "Integer",
  "mfaEnabled": "Boolean"
}
```

