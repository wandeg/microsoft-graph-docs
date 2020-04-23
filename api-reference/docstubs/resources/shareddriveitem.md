---
title: "sharedDriveItem resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# sharedDriveItem resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [baseItem](../resources/baseitem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List sharedDriveItems](../api/shareddriveitem-list.md)|[sharedDriveItem](../resources/shareddriveitem.md) collection|Get a list of the [sharedDriveItem](../resources/shareddriveitem.md) objects and their properties.|
|[Get sharedDriveItem](../api/shareddriveitem-get.md)|[sharedDriveItem](../resources/shareddriveitem.md)|Read the properties and relationships of a [sharedDriveItem](../resources/shareddriveitem.md) object.|
|[Create sharedDriveItem](../api/shareddriveitem-post-shares.md)|[sharedDriveItem](../resources/shareddriveitem.md)|Create a new [sharedDriveItem](../resources/shareddriveitem.md) object.|
|[Delete sharedDriveItem](../api/shareddriveitem-delete.md)|None|Deletes a [sharedDriveItem](../resources/shareddriveitem.md) object.|
|[Update sharedDriveItem](../api/shareddriveitem-update.md)|[sharedDriveItem](../resources/shareddriveitem.md)|Update the properties of a [sharedDriveItem](../resources/shareddriveitem.md) object.|
|[List createdByUser](../api/shareddriveitem-list-createdbyuser.md)|[user](../resources/user.md) collection|Get the users from the createdByUser navigation property.|
|[Add createdByUser](../api/shareddriveitem-post-createdbyuser.md)|[user](../resources/user.md)|Add createdByUser by posting to the createdByUser collection.|
|[Remove createdByUser](../api/shareddriveitem-delete-createdbyuser.md)|None|Remove a [user](../resources/user.md) object.|
|[List lastModifiedByUser](../api/shareddriveitem-list-lastmodifiedbyuser.md)|[user](../resources/user.md) collection|Get the users from the lastModifiedByUser navigation property.|
|[Add lastModifiedByUser](../api/shareddriveitem-post-lastmodifiedbyuser.md)|[user](../resources/user.md)|Add lastModifiedByUser by posting to the lastModifiedByUser collection.|
|[Remove lastModifiedByUser](../api/shareddriveitem-delete-lastmodifiedbyuser.md)|None|Remove a [user](../resources/user.md) object.|
|[List driveItem](../api/shareddriveitem-list-driveitem.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItems from the driveItem navigation property.|
|[Create driveItem](../api/shareddriveitem-post-driveitem.md)|[driveItem](../resources/driveitem.md)|Create a new driveItem object.|
|[Delete driveItem](../api/shareddriveitem-delete-driveitem.md)|None|Delete a [driveItem](../resources/driveitem.md) object.|
|[Update driveItem](../api/shareddriveitem-update-driveitem.md)|[driveItem](../resources/driveitem.md)|Update the properties of a driveItem object.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveitem.md)|Read the properties and relationships of a [driveItem](../resources/driveitem.md) object.|
|[List items](../api/shareddriveitem-list-items.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItems from the items navigation property.|
|[Create items](../api/shareddriveitem-post-items.md)|[driveItem](../resources/driveitem.md)|Create a new items object.|
|[Delete items](../api/shareddriveitem-delete-items.md)|None|Delete an [driveItem](../resources/driveitem.md) object.|
|[Update items](../api/shareddriveitem-update-items.md)|[driveItem](../resources/driveitem.md)|Update the properties of an items object.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveitem.md)|Read the properties and relationships of a [driveItem](../resources/driveitem.md) object.|
|[List list](../api/shareddriveitem-list-list.md)|[list](../resources/list.md) collection|Get the lists from the list navigation property.|
|[Create list](../api/shareddriveitem-post-list.md)|[list](../resources/list.md)|Create a new list object.|
|[Delete list](../api/shareddriveitem-delete-list.md)|None|Delete a [list](../resources/list.md) object.|
|[Update list](../api/shareddriveitem-update-list.md)|[list](../resources/list.md)|Update the properties of a list object.|
|[Get list](../api/list-get.md)|[list](../resources/list.md)|Read the properties and relationships of a [list](../resources/list.md) object.|
|[List listItem](../api/shareddriveitem-list-listitem.md)|[listItem](../resources/listitem.md) collection|Get the listItems from the listItem navigation property.|
|[Create listItem](../api/shareddriveitem-post-listitem.md)|[listItem](../resources/listitem.md)|Create a new listItem object.|
|[Delete listItem](../api/shareddriveitem-delete-listitem.md)|None|Delete a [listItem](../resources/listitem.md) object.|
|[Update listItem](../api/shareddriveitem-update-listitem.md)|[listItem](../resources/listitem.md)|Update the properties of a listItem object.|
|[Get listItem](../api/listitem-get.md)|[listItem](../resources/listitem.md)|Read the properties and relationships of a [listItem](../resources/listitem.md) object.|
|[List root](../api/shareddriveitem-list-root.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItems from the root navigation property.|
|[Create root](../api/shareddriveitem-post-root.md)|[driveItem](../resources/driveitem.md)|Create a new root object.|
|[Delete root](../api/shareddriveitem-delete-root.md)|None|Delete a [driveItem](../resources/driveitem.md) object.|
|[Update root](../api/shareddriveitem-update-root.md)|[driveItem](../resources/driveitem.md)|Update the properties of a root object.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveitem.md)|Read the properties and relationships of a [driveItem](../resources/driveitem.md) object.|
|[List site](../api/shareddriveitem-list-site.md)|[site](../resources/site.md) collection|Get the sites from the site navigation property.|
|[Create site](../api/shareddriveitem-post-site.md)|[site](../resources/site.md)|Create a new site object.|
|[Delete site](../api/shareddriveitem-delete-site.md)|None|Delete a [site](../resources/site.md) object.|
|[Update site](../api/shareddriveitem-update-site.md)|[site](../resources/site.md)|Update the properties of a site object.|
|[Get site](../api/site-get.md)|[site](../resources/site.md)|Read the properties and relationships of a [site](../resources/site.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|description|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|eTag|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|name|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|owner|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|parentReference|[itemReference](../resources/itemreference.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|webUrl|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|createdByUser|[user](../resources/user.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|driveItem|[driveItem](../resources/driveitem.md)|**TODO: Add Description**|
|items|[driveItem](../resources/driveitem.md) collection|**TODO: Add Description**|
|lastModifiedByUser|[user](../resources/user.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|list|[list](../resources/list.md)|**TODO: Add Description**|
|listItem|[listItem](../resources/listitem.md)|**TODO: Add Description**|
|root|[driveItem](../resources/driveitem.md)|**TODO: Add Description**|
|site|[site](../resources/site.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedDriveItem",
  "baseType": "microsoft.graph.baseItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedDriveItem",
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
  "owner": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

