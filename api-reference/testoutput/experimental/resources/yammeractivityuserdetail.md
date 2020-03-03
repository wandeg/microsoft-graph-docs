---
title: "yammerActivityUserDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# yammerActivityUserDetail resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List yammerActivityUserDetails](../api/yammeractivityuserdetail-list.md)|[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md) collection|List properties and relationships of the [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md) objects.|
|[Get yammerActivityUserDetail](../api/yammeractivityuserdetail-get.md)|[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)|Read properties and relationships of the [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md) object.|
|[Create yammerActivityUserDetail](../api/yammeractivityuserdetail-create.md)|[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)|Create a new [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md) object.|
|[Delete yammerActivityUserDetail](../api/yammeractivityuserdetail-delete.md)|None|Deletes a [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md).|
|[Update yammerActivityUserDetail](../api/yammeractivityuserdetail-update.md)|[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)|Update the properties of a [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedProducts|String collection||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastActivityDate|Date||
|likedCount|Int64||
|postedCount|Int64||
|readCount|Int64||
|reportPeriod|String||
|reportRefreshDate|Date||
|stateChangeDate|Date||
|userPrincipalName|String||
|userState|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.yammerActivityUserDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.yammerActivityUserDetail",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "userPrincipalName": "String",
  "displayName": "String",
  "userState": "String",
  "stateChangeDate": "Date",
  "lastActivityDate": "Date",
  "postedCount": 1024,
  "readCount": 1024,
  "likedCount": 1024,
  "assignedProducts": [
    "String"
  ],
  "reportPeriod": "String"
}
```

