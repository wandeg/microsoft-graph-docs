---
title: "teamsUserActivityUserDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# teamsUserActivityUserDetail resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List teamsUserActivityUserDetails](../api/teamsuseractivityuserdetail-list.md)|[teamsUserActivityUserDetail](../resources/teamsUserActivityUserDetail.md) collection|List properties and relationships of the [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) objects.|
|[Get teamsUserActivityUserDetail](../api/teamsuseractivityuserdetail-get.md)|[teamsUserActivityUserDetail](../resources/teamsUserActivityUserDetail.md)|Read properties and relationships of the [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) object.|
|[Create teamsUserActivityUserDetail](../api/teamsuseractivityuserdetail-create.md)|[teamsUserActivityUserDetail](../resources/teamsUserActivityUserDetail.md)|Create a new [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) object.|
|[Delete teamsUserActivityUserDetail](../api/teamsuseractivityuserdetail-delete.md)|None|Deletes a [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md).|
|[Update teamsUserActivityUserDetail](../api/teamsuseractivityuserdetail-update.md)|[teamsUserActivityUserDetail](../resources/teamsUserActivityUserDetail.md)|Update the properties of a [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedProducts|String collection||
|callCount|Int64||
|deletedDate|Date||
|hasOtherAction|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean||
|lastActivityDate|Date||
|meetingCount|Int64||
|privateChatMessageCount|Int64||
|reportPeriod|String||
|reportRefreshDate|Date||
|teamChatMessageCount|Int64||
|userPrincipalName|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsUserActivityUserDetail",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "userPrincipalName": "String",
  "lastActivityDate": "Date",
  "isDeleted": true,
  "deletedDate": "Date",
  "assignedProducts": [
    "String"
  ],
  "teamChatMessageCount": 1024,
  "privateChatMessageCount": 1024,
  "callCount": 1024,
  "meetingCount": 1024,
  "hasOtherAction": true,
  "reportPeriod": "String"
}
```

