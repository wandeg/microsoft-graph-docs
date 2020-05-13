---
title: "drive resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# drive resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [baseItem](../resources/baseitem.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List drive](../api/user-list-drive.md)|[drive](../resources/drive.md) collection|Get the drives from the drive navigation property.|
|[Create drive](../api/user-post-drive.md)|[drive](../resources/drive.md)|Create a new drive object.|
|[Delete drive](../api/user-delete-drive.md)|None|Delete a [drive](../resources/drive.md) object.|
|[Update drive](../api/user-update-drive.md)|[drive](../resources/drive.md)|Update the properties of a drive object.|
|[Get drive](../api/user-get-drive.md)|[drive](../resources/drive.md)|Read the properties and relationships of a [drive](../resources/drive.md) object.|
|[List drives](../api/drive-list.md)|[drive](../resources/drive.md) collection|Get a list of the [drive](../resources/drive.md) objects and their properties.|
|[Get drive](../api/drive-get.md)|[drive](../resources/drive.md)|Read the properties and relationships of a [drive](../resources/drive.md) object.|
|[Create drive](../api/drive-post-drives.md)|[drive](../resources/drive.md)|Create a new [drive](../resources/drive.md) object.|
|[Delete drive](../api/drive-delete.md)|None|Deletes a [drive](../resources/drive.md) object.|
|[Update drive](../api/drive-update.md)|[drive](../resources/drive.md)|Update the properties of a [drive](../resources/drive.md) object.|
|[recent](../api/drive-recent.md)|[driveItem](../resources/driveitem.md) collection|**TODO: Add Description**|
|[search](../api/drive-search.md)|[driveItem](../resources/driveitem.md) collection|**TODO: Add Description**|
|[sharedWithMe](../api/drive-sharedwithme.md)|[driveItem](../resources/driveitem.md) collection|**TODO: Add Description**|
|[List createdByUser](../api/drive-list-createdbyuser.md)|[user](../resources/user.md) collection|Get the users from the createdByUser navigation property.|
|[Add createdByUser](../api/drive-post-createdbyuser.md)|[user](../resources/user.md)|Add createdByUser by posting to the createdByUser collection.|
|[Remove createdByUser](../api/drive-delete-createdbyuser.md)|None|Remove a [user](../resources/user.md) object.|
|[List lastModifiedByUser](../api/drive-list-lastmodifiedbyuser.md)|[user](../resources/user.md) collection|Get the users from the lastModifiedByUser navigation property.|
|[Add lastModifiedByUser](../api/drive-post-lastmodifiedbyuser.md)|[user](../resources/user.md)|Add lastModifiedByUser by posting to the lastModifiedByUser collection.|
|[Remove lastModifiedByUser](../api/drive-delete-lastmodifiedbyuser.md)|None|Remove a [user](../resources/user.md) object.|
|[List following](../api/drive-list-following.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItems from the following navigation property.|
|[Create following](../api/drive-post-following.md)|[driveItem](../resources/driveitem.md)|Create a new following object.|
|[Delete following](../api/drive-delete-following.md)|None|Delete a [driveItem](../resources/driveitem.md) object.|
|[Update following](../api/drive-update-following.md)|[driveItem](../resources/driveitem.md)|Update the properties of a following object.|
|[Get following](../api/drive-get-driveitem.md)|[driveItem](../resources/driveitem.md)|Read the properties and relationships of a [driveItem](../resources/driveitem.md) object.|
|[List items](../api/drive-list-items.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItems from the items navigation property.|
|[Create items](../api/drive-post-items.md)|[driveItem](../resources/driveitem.md)|Create a new items object.|
|[Delete items](../api/drive-delete-items.md)|None|Delete a [driveItem](../resources/driveitem.md) object.|
|[Update items](../api/drive-update-items.md)|[driveItem](../resources/driveitem.md)|Update the properties of an items object.|
|[Get items](../api/drive-get-driveitem.md)|[driveItem](../resources/driveitem.md)|Read the properties and relationships of a [driveItem](../resources/driveitem.md) object.|
|[List list](../api/drive-list-list.md)|[list](../resources/list.md) collection|Get the lists from the list navigation property.|
|[Create list](../api/drive-post-list.md)|[list](../resources/list.md)|Create a new list object.|
|[Delete list](../api/drive-delete-list.md)|None|Delete a [list](../resources/list.md) object.|
|[Update list](../api/drive-update-list.md)|[list](../resources/list.md)|Update the properties of a list object.|
|[Get list](../api/drive-get-list.md)|[list](../resources/list.md)|Read the properties and relationships of a [list](../resources/list.md) object.|
|[List root](../api/drive-list-root.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItems from the root navigation property.|
|[Create root](../api/drive-post-root.md)|[driveItem](../resources/driveitem.md)|Create a new root object.|
|[Delete root](../api/drive-delete-root.md)|None|Delete a [driveItem](../resources/driveitem.md) object.|
|[Update root](../api/drive-update-root.md)|[driveItem](../resources/driveitem.md)|Update the properties of a root object.|
|[Get root](../api/drive-get-driveitem.md)|[driveItem](../resources/driveitem.md)|Read the properties and relationships of a [driveItem](../resources/driveitem.md) object.|
|[List special](../api/drive-list-special.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItems from the special navigation property.|
|[Create special](../api/drive-post-special.md)|[driveItem](../resources/driveitem.md)|Create a new special object.|
|[Delete special](../api/drive-delete-special.md)|None|Delete a [driveItem](../resources/driveitem.md) object.|
|[Update special](../api/drive-update-special.md)|[driveItem](../resources/driveitem.md)|Update the properties of a special object.|
|[Get special](../api/drive-get-driveitem.md)|[driveItem](../resources/driveitem.md)|Read the properties and relationships of a [driveItem](../resources/driveitem.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|description|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|driveType|String|**TODO: Add Description**|
|eTag|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|name|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|owner|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|parentReference|[itemReference](../resources/itemreference.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|quota|[quota](../resources/quota.md)|**TODO: Add Description**|
|sharePointIds|[sharepointIds](../resources/sharepointids.md)|**TODO: Add Description**|
|system|[systemFacet](../resources/systemfacet.md)|**TODO: Add Description**|
|webUrl|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|createdByUser|[user](../resources/user.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|following|[driveItem](../resources/driveitem.md) collection|**TODO: Add Description**|
|items|[driveItem](../resources/driveitem.md) collection|**TODO: Add Description**|
|lastModifiedByUser|[user](../resources/user.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|list|[list](../resources/list.md)|**TODO: Add Description**|
|root|[driveItem](../resources/driveitem.md)|**TODO: Add Description**|
|special|[driveItem](../resources/driveitem.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.quota"
  },
  "sharePointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "system": {
    "@odata.type": "microsoft.graph.systemFacet"
  }
}
```

