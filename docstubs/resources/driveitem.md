---
title: "driveItem resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# driveItem resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [baseItem](../resources/baseitem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List driveItems](../api/driveitem-list.md)|[driveItem](../resources/driveitem.md) collection|Get a list of the [driveItem](../resources/driveitem.md) objects and their properties.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveitem.md)|Read properties and relationships of a [driveItem](../resources/driveitem.md) object.|
|[Create driveItem](../api/driveitem-post-workbooks.md)|[driveItem](../resources/driveitem.md)|Create a new [driveItem](../resources/driveitem.md) object.|
|[Delete driveItem](../api/driveitem-delete.md)|None|Deletes a [driveItem](../resources/driveitem.md).|
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
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of an [user](../resources/user.md) object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of an [user](../resources/user.md) object.|
|[Get workbook](../api/workbook-get.md)|[workbook](../resources/workbook.md)|Read properties and relationships of a [workbook](../resources/workbook.md) object.|
|[List activities](../api/driveitem-list-activities.md)|[itemActivityOLD](../resources/itemactivityold.md) collection|Get the itemActivityOLDs from the activities navigation property.|
|[Add activities](../api/driveitem-post-activities.md)|[itemActivityOLD](../resources/itemactivityold.md)|Add activities by posting to the activities collection.|
|[Get itemAnalytics](../api/itemanalytics-get.md)|[itemAnalytics](../resources/itemanalytics.md)|Read properties and relationships of an [itemAnalytics](../resources/itemanalytics.md) object.|
|[List children](../api/driveitem-list-children.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItems from the children navigation property.|
|[Add children](../api/driveitem-post-children.md)|[driveItem](../resources/driveitem.md)|Add children by posting to the children collection.|
|[Get listItem](../api/listitem-get.md)|[listItem](../resources/listitem.md)|Read properties and relationships of a [listItem](../resources/listitem.md) object.|
|[List permissions](../api/driveitem-list-permissions.md)|[permission](../resources/permission.md) collection|Get the permissions from the permissions navigation property.|
|[Add permissions](../api/driveitem-post-permissions.md)|[permission](../resources/permission.md)|Add permissions by posting to the permissions collection.|
|[List subscriptions](../api/driveitem-list-subscriptions.md)|[subscription](../resources/subscription.md) collection|Get the subscriptions from the subscriptions navigation property.|
|[Add subscriptions](../api/driveitem-post-subscriptions.md)|[subscription](../resources/subscription.md)|Add subscriptions by posting to the subscriptions collection.|
|[List thumbnails](../api/driveitem-list-thumbnails.md)|[thumbnailSet](../resources/thumbnailset.md) collection|Get the thumbnailSets from the thumbnails navigation property.|
|[Add thumbnails](../api/driveitem-post-thumbnails.md)|[thumbnailSet](../resources/thumbnailset.md)|Add thumbnails by posting to the thumbnails collection.|
|[List versions](../api/driveitem-list-versions.md)|[driveItemVersion](../resources/driveitemversion.md) collection|Get the driveItemVersions from the versions navigation property.|
|[Add versions](../api/driveitem-post-versions.md)|[driveItemVersion](../resources/driveitemversion.md)|Add versions by posting to the versions collection.|
|[Get document](../api/document-get.md)|[document](../resources/document.md)|Read properties and relationships of a [document](../resources/document.md) object.|
|[List children](../api/driveitem-list-children.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItems from the children navigation property.|
|[Add children](../api/driveitem-post-children.md)|[driveItem](../resources/driveitem.md)|Add children by posting to the children collection.|

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
|document|[document](../resources/document.md)|**TODO: Add Description**|
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
  "size": 1024,
  "specialFolder": {
    "@odata.type": "microsoft.graph.specialFolder"
  },
  "video": {
    "@odata.type": "microsoft.graph.video"
  },
  "webDavUrl": "String"
}
```

