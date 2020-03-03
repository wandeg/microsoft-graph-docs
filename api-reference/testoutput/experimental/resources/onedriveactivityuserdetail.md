---
title: "oneDriveActivityUserDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# oneDriveActivityUserDetail resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List oneDriveActivityUserDetails](../api/onedriveactivityuserdetail-list.md)|[oneDriveActivityUserDetail](../resources/oneDriveActivityUserDetail.md) collection|List properties and relationships of the [oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md) objects.|
|[Get oneDriveActivityUserDetail](../api/onedriveactivityuserdetail-get.md)|[oneDriveActivityUserDetail](../resources/oneDriveActivityUserDetail.md)|Read properties and relationships of the [oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md) object.|
|[Create oneDriveActivityUserDetail](../api/onedriveactivityuserdetail-create.md)|[oneDriveActivityUserDetail](../resources/oneDriveActivityUserDetail.md)|Create a new [oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md) object.|
|[Delete oneDriveActivityUserDetail](../api/onedriveactivityuserdetail-delete.md)|None|Deletes a [oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md).|
|[Update oneDriveActivityUserDetail](../api/onedriveactivityuserdetail-update.md)|[oneDriveActivityUserDetail](../resources/oneDriveActivityUserDetail.md)|Update the properties of a [oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md) object.|

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

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.oneDriveActivityUserDetail",
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
  "assignedProducts": [
    "String"
  ],
  "reportPeriod": "String"
}
```

