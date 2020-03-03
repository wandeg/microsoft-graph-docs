---
title: "drive resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# drive resource type




Inherits from [baseItem](../resources/baseItem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get drive](../api/drive-get.md)|[drive](../resources/drive.md)|Read properties and relationships of the [drive](../resources/drive.md) object.|
|[Delete drive](../api/drive-delete.md)|None|Deletes a [drive](../resources/drive.md).|
|[Update drive](../api/drive-update.md)|[drive](../resources/drive.md)|Update the properties of a [drive](../resources/drive.md) object.|
|[recent](../api/drive-recent.md)|[driveItem](../resources/driveItem.md) collection||
|[search](../api/drive-search.md)|[driveItem](../resources/driveItem.md) collection||
|[sharedWithMe](../api/drive-sharedwithme.md)|[driveItem](../resources/driveItem.md) collection||
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|
|[List activities](../api/drive-list-activities.md)|[itemActivityOLD](../resources/itemActivityOLD.md) collection|Get the itemActivityOLDs from the activities navigation property.|
|[Add activities](../api/drive-post-activities.md)|[itemActivityOLD](../resources/itemActivityOLD.md)|Add activities by posting to the activities collection.|
|[List bundles](../api/drive-list-bundles.md)|[driveItem](../resources/driveItem.md) collection|Get the driveItems from the bundles navigation property.|
|[Add bundles](../api/drive-post-bundles.md)|[driveItem](../resources/driveItem.md)|Add bundles by posting to the bundles collection.|
|[List following](../api/drive-list-following.md)|[driveItem](../resources/driveItem.md) collection|Get the driveItems from the following navigation property.|
|[Add following](../api/drive-post-following.md)|[driveItem](../resources/driveItem.md)|Add following by posting to the following collection.|
|[List items](../api/drive-list-items.md)|[driveItem](../resources/driveItem.md) collection|Get the driveItems from the items navigation property.|
|[Add items](../api/drive-post-items.md)|[driveItem](../resources/driveItem.md)|Add items by posting to the items collection.|
|[Get list](../api/list-get.md)|[list](../resources/list.md)|Read properties and relationships of the [list](../resources/list.md) object.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveItem.md)|Read properties and relationships of the [driveItem](../resources/driveitem.md) object.|
|[List special](../api/drive-list-special.md)|[driveItem](../resources/driveItem.md) collection|Get the driveItems from the special navigation property.|
|[Add special](../api/drive-post-special.md)|[driveItem](../resources/driveItem.md)|Add special by posting to the special collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identitySet.md)| Inherited from [baseItem](../resources/baseItem.md)|
|createdDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseItem.md)|
|description|String| Inherited from [baseItem](../resources/baseItem.md)|
|driveType|String||
|eTag|String| Inherited from [baseItem](../resources/baseItem.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [baseItem](../resources/baseItem.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseItem.md)|
|name|String| Inherited from [baseItem](../resources/baseItem.md)|
|owner|[identitySet](../resources/identitySet.md)||
|parentReference|[itemReference](../resources/itemReference.md)| Inherited from [baseItem](../resources/baseItem.md)|
|quota|[quota](../resources/quota.md)||
|sharePointIds|[sharepointIds](../resources/sharepointIds.md)||
|system|[systemFacet](../resources/systemFacet.md)||
|webUrl|String| Inherited from [baseItem](../resources/baseItem.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|activities|[itemActivityOLD](../resources/itemActivityOLD.md) collection||
|bundles|[driveItem](../resources/driveItem.md) collection||
|createdByUser|[user](../resources/user.md)| Inherited from [baseItem](../resources/baseItem.md)|
|following|[driveItem](../resources/driveItem.md) collection||
|items|[driveItem](../resources/driveItem.md) collection||
|lastModifiedByUser|[user](../resources/user.md)| Inherited from [baseItem](../resources/baseItem.md)|
|list|[list](../resources/list.md)||
|root|[driveItem](../resources/driveItem.md)||
|special|[driveItem](../resources/driveItem.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.drive",
  "baseType": "microsoft.graph.baseItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.drive",
  "id": "String (identifier)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "eTag": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference"
  },
  "webUrl": "String",
  "driveType": "String",
  "owner": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "quota": {
    "@odata.type": "microsoft.graph.quota",
    "deleted": 1024,
    "remaining": 1024,
    "total": 1024,
    "used": 1024,
    "storagePlanInformation": {
      "@odata.type": "microsoft.graph.storagePlanInformation",
      "upgradeAvailable": true
    }
  },
  "sharePointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "system": {
    "@odata.type": "microsoft.graph.systemFacet"
  }
}
```

