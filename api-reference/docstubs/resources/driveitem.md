---
title: "driveItem resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# driveItem resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [baseItem](../resources/baseitem.md)

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List driveItems](../api/driveitem-list.md)|[driveItem](../resources/driveitem.md) collection|Get a list of the [driveItem](../resources/driveitem.md) objects and their properties.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveitem.md)|Read the properties and relationships of a [driveItem](../resources/driveitem.md) object.|
|[Create driveItem](../api/driveitem-post-workbooks.md)|[driveItem](../resources/driveitem.md)|Create a new [driveItem](../resources/driveitem.md) object.|
|[Delete driveItem](../api/driveitem-delete.md)|None|Deletes a [driveItem](../resources/driveitem.md) object.|
|[Update driveItem](../api/driveitem-update.md)|[driveItem](../resources/driveitem.md)|Update the properties of a [driveItem](../resources/driveitem.md) object.|
|[delta](../api/driveitem-delta.md)|[driveItem](../resources/driveitem.md) collection|**TODO: Add Description**|
|[delta](../api/driveitem-delta.md)|[driveItem](../resources/driveitem.md) collection|**TODO: Add Description**|
|[getActivitiesByInterval](../api/driveitem-getactivitiesbyinterval.md)|[itemActivityStat](../resources/itemactivitystat.md) collection|**TODO: Add Description**|
|[search](../api/driveitem-search.md)|[driveItem](../resources/driveitem.md) collection|**TODO: Add Description**|
|[checkin](../api/driveitem-checkin.md)|None|**TODO: Add Description**|
|[checkout](../api/driveitem-checkout.md)|None|**TODO: Add Description**|
|[copy](../api/driveitem-copy.md)|[driveItem](../resources/driveitem.md)|**TODO: Add Description**|
|[createLink](../api/driveitem-createlink.md)|[permission](../resources/permission.md)|**TODO: Add Description**|
|[createUploadSession](../api/driveitem-createuploadsession.md)|[uploadSession](../resources/uploadsession.md)|**TODO: Add Description**|
|[follow](../api/driveitem-follow.md)|[driveItem](../resources/driveitem.md)|**TODO: Add Description**|
|[unfollow](../api/driveitem-unfollow.md)|None|**TODO: Add Description**|
|[invite](../api/driveitem-invite.md)|[permission](../resources/permission.md) collection|**TODO: Add Description**|
|[preview](../api/driveitem-preview.md)|[itemPreviewInfo](../resources/itempreviewinfo.md)|**TODO: Add Description**|
|[restore](../api/driveitem-restore.md)|[driveItem](../resources/driveitem.md)|**TODO: Add Description**|
|[validatePermission](../api/driveitem-validatepermission.md)|None|**TODO: Add Description**|
|[List createdByUser](../api/driveitem-list-createdbyuser.md)|[user](../resources/user.md) collection|Get the users from the createdByUser navigation property.|
|[Add createdByUser](../api/driveitem-post-createdbyuser.md)|[user](../resources/user.md)|Add createdByUser by posting to the createdByUser collection.|
|[Remove createdByUser](../api/driveitem-delete-createdbyuser.md)|None|Remove a [user](../resources/user.md) object.|
|[List lastModifiedByUser](../api/driveitem-list-lastmodifiedbyuser.md)|[user](../resources/user.md) collection|Get the users from the lastModifiedByUser navigation property.|
|[Add lastModifiedByUser](../api/driveitem-post-lastmodifiedbyuser.md)|[user](../resources/user.md)|Add lastModifiedByUser by posting to the lastModifiedByUser collection.|
|[Remove lastModifiedByUser](../api/driveitem-delete-lastmodifiedbyuser.md)|None|Remove a [user](../resources/user.md) object.|
|[List workbook](../api/driveitem-list-workbook.md)|[workbook](../resources/workbook.md) collection|Get the workbooks from the workbook navigation property.|
|[Create workbook](../api/driveitem-post-workbook.md)|[workbook](../resources/workbook.md)|Create a new workbook object.|
|[Delete workbook](../api/driveitem-delete-workbook.md)|None|Delete a [workbook](../resources/workbook.md) object.|
|[Update workbook](../api/driveitem-update-workbook.md)|[workbook](../resources/workbook.md)|Update the properties of a workbook object.|
|[Get workbook](../api/workbook-get.md)|[workbook](../resources/workbook.md)|Read the properties and relationships of a [workbook](../resources/workbook.md) object.|
|[List activities](../api/driveitem-list-activities.md)|[itemActivityOLD](../resources/itemactivityold.md) collection|Get the itemActivityOLDs from the activities navigation property.|
|[Create activities](../api/driveitem-post-activities.md)|[itemActivityOLD](../resources/itemactivityold.md)|Create a new activities object.|
|[Delete activities](../api/driveitem-delete-activities.md)|None|Delete an [itemActivityOLD](../resources/itemactivityold.md) object.|
|[Update activities](../api/driveitem-update-activities.md)|[itemActivityOLD](../resources/itemactivityold.md)|Update the properties of an activities object.|
|[Get itemActivityOLD](../api/itemactivityold-get.md)|[itemActivityOLD](../resources/itemactivityold.md)|Read the properties and relationships of an [itemActivityOLD](../resources/itemactivityold.md) object.|
|[List analytics](../api/driveitem-list-analytics.md)|[itemAnalytics](../resources/itemanalytics.md) collection|Get the itemAnalytics from the analytics navigation property.|
|[Add analytics](../api/driveitem-post-analytics.md)|[itemAnalytics](../resources/itemanalytics.md)|Add analytics by posting to the analytics collection.|
|[Remove analytics](../api/driveitem-delete-analytics.md)|None|Remove an [itemAnalytics](../resources/itemanalytics.md) object.|
|[List children](../api/driveitem-list-children.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItems from the children navigation property.|
|[Create children](../api/driveitem-post-children.md)|[driveItem](../resources/driveitem.md)|Create a new children object.|
|[Delete children](../api/driveitem-delete-children.md)|None|Delete a [driveItem](../resources/driveitem.md) object.|
|[Update children](../api/driveitem-update-children.md)|[driveItem](../resources/driveitem.md)|Update the properties of a children object.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveitem.md)|Read the properties and relationships of a [driveItem](../resources/driveitem.md) object.|
|[List listItem](../api/driveitem-list-listitem.md)|[listItem](../resources/listitem.md) collection|Get the listItems from the listItem navigation property.|
|[Create listItem](../api/driveitem-post-listitem.md)|[listItem](../resources/listitem.md)|Create a new listItem object.|
|[Delete listItem](../api/driveitem-delete-listitem.md)|None|Delete a [listItem](../resources/listitem.md) object.|
|[Update listItem](../api/driveitem-update-listitem.md)|[listItem](../resources/listitem.md)|Update the properties of a listItem object.|
|[Get listItem](../api/listitem-get.md)|[listItem](../resources/listitem.md)|Read the properties and relationships of a [listItem](../resources/listitem.md) object.|
|[List permissions](../api/driveitem-list-permissions.md)|[permission](../resources/permission.md) collection|Get the permissions from the permissions navigation property.|
|[Create permissions](../api/driveitem-post-permissions.md)|[permission](../resources/permission.md)|Create a new permissions object.|
|[Delete permissions](../api/driveitem-delete-permissions.md)|None|Delete a [permission](../resources/permission.md) object.|
|[Update permissions](../api/driveitem-update-permissions.md)|[permission](../resources/permission.md)|Update the properties of a permissions object.|
|[Get permission](../api/permission-get.md)|[permission](../resources/permission.md)|Read the properties and relationships of a [permission](../resources/permission.md) object.|
|[List subscriptions](../api/driveitem-list-subscriptions.md)|[subscription](../resources/subscription.md) collection|Get the subscriptions from the subscriptions navigation property.|
|[Create subscriptions](../api/driveitem-post-subscriptions.md)|[subscription](../resources/subscription.md)|Create a new subscriptions object.|
|[Delete subscriptions](../api/driveitem-delete-subscriptions.md)|None|Delete a [subscription](../resources/subscription.md) object.|
|[Update subscriptions](../api/driveitem-update-subscriptions.md)|[subscription](../resources/subscription.md)|Update the properties of a subscriptions object.|
|[Get subscription](../api/subscription-get.md)|[subscription](../resources/subscription.md)|Read the properties and relationships of a [subscription](../resources/subscription.md) object.|
|[List thumbnails](../api/driveitem-list-thumbnails.md)|[thumbnailSet](../resources/thumbnailset.md) collection|Get the thumbnailSets from the thumbnails navigation property.|
|[Create thumbnails](../api/driveitem-post-thumbnails.md)|[thumbnailSet](../resources/thumbnailset.md)|Create a new thumbnails object.|
|[Delete thumbnails](../api/driveitem-delete-thumbnails.md)|None|Delete a [thumbnailSet](../resources/thumbnailset.md) object.|
|[Update thumbnails](../api/driveitem-update-thumbnails.md)|[thumbnailSet](../resources/thumbnailset.md)|Update the properties of a thumbnails object.|
|[Get thumbnailSet](../api/thumbnailset-get.md)|[thumbnailSet](../resources/thumbnailset.md)|Read the properties and relationships of a [thumbnailSet](../resources/thumbnailset.md) object.|
|[List versions](../api/driveitem-list-versions.md)|[driveItemVersion](../resources/driveitemversion.md) collection|Get the driveItemVersions from the versions navigation property.|
|[Create versions](../api/driveitem-post-versions.md)|[driveItemVersion](../resources/driveitemversion.md)|Create a new versions object.|
|[Delete versions](../api/driveitem-delete-versions.md)|None|Delete a [driveItemVersion](../resources/driveitemversion.md) object.|
|[Update versions](../api/driveitem-update-versions.md)|[driveItemVersion](../resources/driveitemversion.md)|Update the properties of a versions object.|
|[Get driveItemVersion](../api/driveitemversion-get.md)|[driveItemVersion](../resources/driveitemversion.md)|Read the properties and relationships of a [driveItemVersion](../resources/driveitemversion.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|audio|[audio](../resources/audio.md)|**TODO: Add Description**|
|bundle|[bundle](../resources/bundle.md)|**TODO: Add Description**|
|content|Stream|**TODO: Add Description**|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|cTag|String|**TODO: Add Description**|
|deleted|[deleted](../resources/deleted.md)|**TODO: Add Description**|
|description|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|eTag|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|file|[file](../resources/file.md)|**TODO: Add Description**|
|fileSystemInfo|[fileSystemInfo](../resources/filesysteminfo.md)|**TODO: Add Description**|
|folder|[folder](../resources/folder.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|image|[image](../resources/image.md)|**TODO: Add Description**|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|location|[geoCoordinates](../resources/geocoordinates.md)|**TODO: Add Description**|
|name|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|package|[package](../resources/package.md)|**TODO: Add Description**|
|parentReference|[itemReference](../resources/itemreference.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|pendingOperations|[pendingOperations](../resources/pendingoperations.md)|**TODO: Add Description**|
|photo|[photo](../resources/photo.md)|**TODO: Add Description**|
|publication|[publicationFacet](../resources/publicationfacet.md)|**TODO: Add Description**|
|remoteItem|[remoteItem](../resources/remoteitem.md)|**TODO: Add Description**|
|root|[root](../resources/root.md)|**TODO: Add Description**|
|searchResult|[searchResult](../resources/searchresult.md)|**TODO: Add Description**|
|shared|[shared](../resources/shared.md)|**TODO: Add Description**|
|sharepointIds|[sharepointIds](../resources/sharepointids.md)|**TODO: Add Description**|
|size|Int64|**TODO: Add Description**|
|specialFolder|[specialFolder](../resources/specialfolder.md)|**TODO: Add Description**|
|video|[video](../resources/video.md)|**TODO: Add Description**|
|webDavUrl|String|**TODO: Add Description**|
|webUrl|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|activities|[itemActivityOLD](../resources/itemactivityold.md) collection|**TODO: Add Description**|
|analytics|[itemAnalytics](../resources/itemanalytics.md)|**TODO: Add Description**|
|children|[driveItem](../resources/driveitem.md) collection|**TODO: Add Description**|
|createdByUser|[user](../resources/user.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedByUser|[user](../resources/user.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|listItem|[listItem](../resources/listitem.md)|**TODO: Add Description**|
|permissions|[permission](../resources/permission.md) collection|**TODO: Add Description**|
|subscriptions|[subscription](../resources/subscription.md) collection|**TODO: Add Description**|
|thumbnails|[thumbnailSet](../resources/thumbnailset.md) collection|**TODO: Add Description**|
|versions|[driveItemVersion](../resources/driveitemversion.md) collection|**TODO: Add Description**|
|workbook|[workbook](../resources/workbook.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.driveItem",
  "baseType": "microsoft.graph.baseItem",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.driveItem",
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
  "audio": {
    "@odata.type": "microsoft.graph.audio"
  },
  "bundle": {
    "@odata.type": "microsoft.graph.bundle"
  },
  "content": "Stream",
  "cTag": "String",
  "deleted": {
    "@odata.type": "microsoft.graph.deleted"
  },
  "file": {
    "@odata.type": "microsoft.graph.file"
  },
  "fileSystemInfo": {
    "@odata.type": "microsoft.graph.fileSystemInfo"
  },
  "folder": {
    "@odata.type": "microsoft.graph.folder"
  },
  "image": {
    "@odata.type": "microsoft.graph.image"
  },
  "location": {
    "@odata.type": "microsoft.graph.geoCoordinates"
  },
  "package": {
    "@odata.type": "microsoft.graph.package"
  },
  "pendingOperations": {
    "@odata.type": "microsoft.graph.pendingOperations"
  },
  "photo": {
    "@odata.type": "microsoft.graph.photo"
  },
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet"
  },
  "remoteItem": {
    "@odata.type": "microsoft.graph.remoteItem"
  },
  "root": {
    "@odata.type": "microsoft.graph.root"
  },
  "searchResult": {
    "@odata.type": "microsoft.graph.searchResult"
  },
  "shared": {
    "@odata.type": "microsoft.graph.shared"
  },
  "sharepointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "size": "Integer",
  "specialFolder": {
    "@odata.type": "microsoft.graph.specialFolder"
  },
  "video": {
    "@odata.type": "microsoft.graph.video"
  },
  "webDavUrl": "String"
}
```

