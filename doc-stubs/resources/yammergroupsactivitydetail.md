---
title: "yammerGroupsActivityDetail resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# yammerGroupsActivityDetail resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|groupDisplayName|String|**TODO: Add Description**|
|groupType|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean|**TODO: Add Description**|
|lastActivityDate|Date|**TODO: Add Description**|
|likedCount|Int64|**TODO: Add Description**|
|memberCount|Int64|**TODO: Add Description**|
|networkDisplayName|String|**TODO: Add Description**|
|office365Connected|Boolean|**TODO: Add Description**|
|ownerPrincipalName|String|**TODO: Add Description**|
|postedCount|Int64|**TODO: Add Description**|
|readCount|Int64|**TODO: Add Description**|
|reportPeriod|String|**TODO: Add Description**|
|reportRefreshDate|Date|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.yammerGroupsActivityDetail",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "groupDisplayName": "String",
  "isDeleted": "Boolean",
  "ownerPrincipalName": "String",
  "lastActivityDate": "Date",
  "groupType": "String",
  "office365Connected": "Boolean",
  "memberCount": "Integer",
  "postedCount": "Integer",
  "readCount": "Integer",
  "likedCount": "Integer",
  "networkDisplayName": "String",
  "reportPeriod": "String"
}
```

