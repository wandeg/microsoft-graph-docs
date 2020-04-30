---
title: "request resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# request resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[stop](../api/request-stop.md)|None|**TODO: Add Description**|
|[recordDecisions](../api/request-recorddecisions.md)|None|**TODO: Add Description**|
|[List approval](../api/request-list-approval.md)|[approval](../resources/approval.md) collection|Get the approvals from the approval navigation property.|
|[Create approval](../api/request-post-approval.md)|[approval](../resources/approval.md)|Create a new approval object.|
|[Delete approval](../api/request-delete-approval.md)|None|Delete an [approval](../resources/approval.md) object.|
|[Update approval](../api/request-update-approval.md)|[approval](../resources/approval.md)|Update the properties of an approval object.|
|[Get approval](../api/approval-get.md)|[approval](../resources/approval.md)|Read the properties and relationships of an [approval](../resources/approval.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|approval|[approval](../resources/approval.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.request",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.request",
  "id": "String (identifier)"
}
```

