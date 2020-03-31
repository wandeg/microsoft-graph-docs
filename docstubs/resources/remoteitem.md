---
title: "remoteItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# remoteItem resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)||
|createdDateTime|DateTimeOffset||
|file|[file](../resources/file.md)||
|fileSystemInfo|[fileSystemInfo](../resources/filesysteminfo.md)||
|folder|[folder](../resources/folder.md)||
|id|String||
|image|[image](../resources/image.md)||
|lastModifiedBy|[identitySet](../resources/identityset.md)||
|lastModifiedDateTime|DateTimeOffset||
|name|String||
|package|[package](../resources/package.md)||
|parentReference|[itemReference](../resources/itemreference.md)||
|shared|[shared](../resources/shared.md)||
|sharepointIds|[sharepointIds](../resources/sharepointids.md)||
|size|Int64||
|specialFolder|[specialFolder](../resources/specialfolder.md)||
|video|[video](../resources/video.md)||
|webDavUrl|String||
|webUrl|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.remoteItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteItem",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "createdDateTime": "String (timestamp)",
  "file": {
    "@odata.type": "microsoft.graph.file",
    "hashes": {
      "@odata.type": "microsoft.graph.hashes",
      "crc32Hash": "String",
      "quickXorHash": "String",
      "sha1Hash": "String",
      "sha256Hash": "String"
    },
    "mimeType": "String",
    "processingMetadata": true
  },
  "fileSystemInfo": {
    "@odata.type": "microsoft.graph.fileSystemInfo",
    "lastAccessedDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
  },
  "folder": {
    "@odata.type": "microsoft.graph.folder",
    "childCount": 1024,
    "view": {
      "@odata.type": "microsoft.graph.folderView",
      "sortBy": "String",
      "sortOrder": "String",
      "viewType": "String"
    }
  },
  "id": "String (identifier)",
  "image": {
    "@odata.type": "microsoft.graph.image",
    "height": 1024,
    "width": 1024
  },
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "package": {
    "@odata.type": "microsoft.graph.package",
    "type": "String"
  },
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference",
    "driveId": "String",
    "driveType": "String",
    "path": "String",
    "shareId": "String",
    "sharepointIds": {
      "@odata.type": "microsoft.graph.sharepointIds",
      "listId": "String",
      "listItemId": "String",
      "listItemUniqueId": "String",
      "siteId": "String",
      "siteUrl": "String",
      "tenantId": "String",
      "webId": "String"
    }
  },
  "shared": {
    "@odata.type": "microsoft.graph.shared",
    "owner": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "scope": "String",
    "sharedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "sharedDateTime": "String (timestamp)"
  },
  "sharepointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "size": 1024,
  "specialFolder": {
    "@odata.type": "microsoft.graph.specialFolder"
  },
  "video": {
    "@odata.type": "microsoft.graph.video",
    "audioBitsPerSample": 1024,
    "audioChannels": 1024,
    "audioFormat": "String",
    "audioSamplesPerSecond": 1024,
    "bitrate": 1024,
    "duration": 1024,
    "fourCC": "String",
    "frameRate": "Double"
  },
  "webDavUrl": "String",
  "webUrl": "String"
}
```

