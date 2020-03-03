---
title: "sharePointActivityUserDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# sharePointActivityUserDetail resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List sharePointActivityUserDetails](../api/sharepointactivityuserdetail-list.md)|[sharePointActivityUserDetail](../resources/sharePointActivityUserDetail.md) collection|List properties and relationships of the [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md) objects.|
|[Get sharePointActivityUserDetail](../api/sharepointactivityuserdetail-get.md)|[sharePointActivityUserDetail](../resources/sharePointActivityUserDetail.md)|Read properties and relationships of the [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md) object.|
|[Create sharePointActivityUserDetail](../api/sharepointactivityuserdetail-create.md)|[sharePointActivityUserDetail](../resources/sharePointActivityUserDetail.md)|Create a new [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md) object.|
|[Delete sharePointActivityUserDetail](../api/sharepointactivityuserdetail-delete.md)|None|Deletes a [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md).|
|[Update sharePointActivityUserDetail](../api/sharepointactivityuserdetail-update.md)|[sharePointActivityUserDetail](../resources/sharePointActivityUserDetail.md)|Update the properties of a [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedProducts|String collection||
|deletedDate|Date||
|id|String| Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean||
|lastActivityDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|sharedExternallyFileCount|Int64||
|sharedInternallyFileCount|Int64||
|syncedFileCount|Int64||
|userPrincipalName|String||
|viewedOrEditedFileCount|Int64||
|visitedPageCount|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharePointActivityUserDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharePointActivityUserDetail",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "userPrincipalName": "String",
  "isDeleted": true,
  "deletedDate": "Date",
  "lastActivityDate": "Date",
  "viewedOrEditedFileCount": 1024,
  "syncedFileCount": 1024,
  "sharedInternallyFileCount": 1024,
  "sharedExternallyFileCount": 1024,
  "visitedPageCount": 1024,
  "assignedProducts": [
    "String"
  ],
  "reportPeriod": "String"
}
```

