---
title: "emailActivityUserDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# emailActivityUserDetail resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List emailActivityUserDetails](../api/emailactivityuserdetail-list.md)|[emailActivityUserDetail](../resources/emailActivityUserDetail.md) collection|List properties and relationships of the [emailActivityUserDetail](../resources/emailactivityuserdetail.md) objects.|
|[Get emailActivityUserDetail](../api/emailactivityuserdetail-get.md)|[emailActivityUserDetail](../resources/emailActivityUserDetail.md)|Read properties and relationships of the [emailActivityUserDetail](../resources/emailactivityuserdetail.md) object.|
|[Create emailActivityUserDetail](../api/emailactivityuserdetail-create.md)|[emailActivityUserDetail](../resources/emailActivityUserDetail.md)|Create a new [emailActivityUserDetail](../resources/emailactivityuserdetail.md) object.|
|[Delete emailActivityUserDetail](../api/emailactivityuserdetail-delete.md)|None|Deletes a [emailActivityUserDetail](../resources/emailactivityuserdetail.md).|
|[Update emailActivityUserDetail](../api/emailactivityuserdetail-update.md)|[emailActivityUserDetail](../resources/emailActivityUserDetail.md)|Update the properties of a [emailActivityUserDetail](../resources/emailactivityuserdetail.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedProducts|String collection||
|deletedDate|Date||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean||
|lastActivityDate|Date||
|readCount|Int64||
|receiveCount|Int64||
|reportPeriod|String||
|reportRefreshDate|Date||
|sendCount|Int64||
|userPrincipalName|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailActivityUserDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.emailActivityUserDetail",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "userPrincipalName": "String",
  "displayName": "String",
  "isDeleted": true,
  "deletedDate": "Date",
  "lastActivityDate": "Date",
  "sendCount": 1024,
  "receiveCount": 1024,
  "readCount": 1024,
  "assignedProducts": [
    "String"
  ],
  "reportPeriod": "String"
}
```

