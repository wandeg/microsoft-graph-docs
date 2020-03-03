---
title: "yammerGroupsActivityDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# yammerGroupsActivityDetail resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List yammerGroupsActivityDetails](../api/yammergroupsactivitydetail-list.md)|[yammerGroupsActivityDetail](../resources/yammerGroupsActivityDetail.md) collection|List properties and relationships of the [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) objects.|
|[Get yammerGroupsActivityDetail](../api/yammergroupsactivitydetail-get.md)|[yammerGroupsActivityDetail](../resources/yammerGroupsActivityDetail.md)|Read properties and relationships of the [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) object.|
|[Create yammerGroupsActivityDetail](../api/yammergroupsactivitydetail-create.md)|[yammerGroupsActivityDetail](../resources/yammerGroupsActivityDetail.md)|Create a new [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) object.|
|[Delete yammerGroupsActivityDetail](../api/yammergroupsactivitydetail-delete.md)|None|Deletes a [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md).|
|[Update yammerGroupsActivityDetail](../api/yammergroupsactivitydetail-update.md)|[yammerGroupsActivityDetail](../resources/yammerGroupsActivityDetail.md)|Update the properties of a [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|groupDisplayName|String||
|groupType|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean||
|lastActivityDate|Date||
|likedCount|Int64||
|memberCount|Int64||
|office365Connected|Boolean||
|ownerPrincipalName|String||
|postedCount|Int64||
|readCount|Int64||
|reportPeriod|String||
|reportRefreshDate|Date||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
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
  "isDeleted": true,
  "ownerPrincipalName": "String",
  "lastActivityDate": "Date",
  "groupType": "String",
  "office365Connected": true,
  "memberCount": 1024,
  "postedCount": 1024,
  "readCount": 1024,
  "likedCount": 1024,
  "reportPeriod": "String"
}
```

