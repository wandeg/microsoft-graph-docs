---
title: "remoteItem resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# remoteItem resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|file|[file](../resources/file.md)|**TODO: Add Description**|
|fileSystemInfo|[fileSystemInfo](../resources/filesysteminfo.md)|**TODO: Add Description**|
|folder|[folder](../resources/folder.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|image|[image](../resources/image.md)|**TODO: Add Description**|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|package|[package](../resources/package.md)|**TODO: Add Description**|
|parentReference|[itemReference](../resources/itemreference.md)|**TODO: Add Description**|
|shared|[shared](../resources/shared.md)|**TODO: Add Description**|
|sharepointIds|[sharepointIds](../resources/sharepointids.md)|**TODO: Add Description**|
|size|Int64|**TODO: Add Description**|
|specialFolder|[specialFolder](../resources/specialfolder.md)|**TODO: Add Description**|
|video|[video](../resources/video.md)|**TODO: Add Description**|
|webDavUrl|String|**TODO: Add Description**|
|webUrl|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.remoteItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteItem",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "file": {
    "@odata.type": "microsoft.graph.file"
  },
  "fileSystemInfo": {
    "@odata.type": "microsoft.graph.fileSystemInfo"
  },
  "folder": {
    "@odata.type": "microsoft.graph.folder"
  },
  "id": "String (identifier)",
  "image": {
    "@odata.type": "microsoft.graph.image"
  },
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "package": {
    "@odata.type": "microsoft.graph.package"
  },
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference"
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
  "webDavUrl": "String",
  "webUrl": "String"
}
```

