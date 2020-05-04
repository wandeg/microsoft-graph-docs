---
title: "Create children"
description: "Create a new children object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create children

Namespace: microsoft.graph

Create a new children object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /workbooks/{workbooksId}/children
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [driveItem](../resources/driveitem.md) object.

The following table shows the properties that are required when you create the [driveItem](../resources/driveitem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|description|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|eTag|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|name|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|parentReference|[itemReference](../resources/itemreference.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|webUrl|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|audio|[audio](../resources/audio.md)|**TODO: Add Description**|
|bundle|[bundle](../resources/bundle.md)|**TODO: Add Description**|
|content|Stream|**TODO: Add Description**|
|cTag|String|**TODO: Add Description**|
|deleted|[deleted](../resources/deleted.md)|**TODO: Add Description**|
|file|[file](../resources/file.md)|**TODO: Add Description**|
|fileSystemInfo|[fileSystemInfo](../resources/filesysteminfo.md)|**TODO: Add Description**|
|folder|[folder](../resources/folder.md)|**TODO: Add Description**|
|image|[image](../resources/image.md)|**TODO: Add Description**|
|location|[geoCoordinates](../resources/geocoordinates.md)|**TODO: Add Description**|
|package|[package](../resources/package.md)|**TODO: Add Description**|
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



## Response
If successful, this method returns a `201 Created` response code and a [driveItem](../resources/driveitem.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_driveitem_from_workbooks"
}
-->
``` http
POST https://graph.microsoft.com/beta/workbooks/{workbooksId}/children
Content-Type: application/json
Content-length: 5211

{
  "@odata.type": "#microsoft.graph.driveItem",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "description": "Description value",
  "eTag": "ETag value",
  "name": "Name value",
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference",
    "driveId": "Drive Id value",
    "driveType": "Drive Type value",
    "path": "Path value",
    "shareId": "Share Id value",
    "sharepointIds": {
      "@odata.type": "microsoft.graph.sharepointIds",
      "listId": "List Id value",
      "listItemId": "List Item Id value",
      "listItemUniqueId": "List Item Unique Id value",
      "siteId": "Site Id value",
      "siteUrl": "https://example.com/siteUrl/",
      "tenantId": "Tenant Id value",
      "webId": "Web Id value"
    }
  },
  "webUrl": "https://example.com/webUrl/",
  "audio": {
    "@odata.type": "microsoft.graph.audio",
    "album": "Album value",
    "albumArtist": "Album Artist value",
    "artist": "Artist value",
    "bitrate": 7,
    "composers": "Composers value",
    "copyright": "Copyright value",
    "disc": 4,
    "discCount": 9,
    "duration": 8,
    "genre": "Genre value",
    "hasDrm": true,
    "isVariableBitrate": true,
    "title": "Title value",
    "track": 5,
    "trackCount": 10,
    "year": 4
  },
  "bundle": {
    "@odata.type": "microsoft.graph.bundle",
    "childCount": 10,
    "album": {
      "@odata.type": "microsoft.graph.album",
      "coverImageItemId": "Cover Image Item Id value"
    }
  },
  "content": "Stream",
  "cTag": "CTag value",
  "deleted": {
    "@odata.type": "microsoft.graph.deleted",
    "state": "State value"
  },
  "file": {
    "@odata.type": "microsoft.graph.file",
    "hashes": {
      "@odata.type": "microsoft.graph.hashes",
      "crc32Hash": "Crc32Hash value",
      "quickXorHash": "Quick Xor Hash value",
      "sha1Hash": "Sha1Hash value",
      "sha256Hash": "Sha256Hash value"
    },
    "mimeType": "Mime Type value",
    "processingMetadata": true
  },
  "fileSystemInfo": {
    "@odata.type": "microsoft.graph.fileSystemInfo",
    "lastAccessedDateTime": "2017-01-01T00:01:56.0899806+03:00"
  },
  "folder": {
    "@odata.type": "microsoft.graph.folder",
    "view": {
      "@odata.type": "microsoft.graph.folderView",
      "sortBy": "Sort By value",
      "sortOrder": "Sort Order value",
      "viewType": "View Type value"
    }
  },
  "image": {
    "@odata.type": "microsoft.graph.image",
    "height": 6,
    "width": 5
  },
  "location": {
    "@odata.type": "microsoft.graph.geoCoordinates",
    "altitude": "Double",
    "latitude": "Double",
    "longitude": "Double"
  },
  "package": {
    "@odata.type": "microsoft.graph.package",
    "type": "Type value"
  },
  "pendingOperations": {
    "@odata.type": "microsoft.graph.pendingOperations",
    "pendingContentUpdate": {
      "@odata.type": "microsoft.graph.pendingContentUpdate",
      "queuedDateTime": "2016-12-31T23:59:00.2417573+03:00"
    }
  },
  "photo": {
    "@odata.type": "microsoft.graph.photo",
    "cameraMake": "Camera Make value",
    "cameraModel": "Camera Model value",
    "exposureDenominator": "Double",
    "exposureNumerator": "Double",
    "fNumber": "Double",
    "focalLength": "Double",
    "iso": 3,
    "orientation": 11,
    "takenDateTime": "2016-12-31T23:58:34.3648434+03:00"
  },
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet",
    "level": "Level value",
    "versionId": "Version Id value"
  },
  "remoteItem": {
    "@odata.type": "microsoft.graph.remoteItem",
    "shared": {
      "@odata.type": "microsoft.graph.shared",
      "owner": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "scope": "Scope value",
      "sharedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "sharedDateTime": "2016-12-31T23:59:32.0800584+03:00"
    },
    "size": 4,
    "specialFolder": {
      "@odata.type": "microsoft.graph.specialFolder"
    },
    "webDavUrl": "https://example.com/webDavUrl/"
  },
  "root": {
    "@odata.type": "microsoft.graph.root"
  },
  "searchResult": {
    "@odata.type": "microsoft.graph.searchResult",
    "onClickTelemetryUrl": "https://example.com/onClickTelemetryUrl/"
  },
  "shared": {
    "@odata.type": "microsoft.graph.shared"
  },
  "sharepointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "size": 4,
  "specialFolder": {
    "@odata.type": "microsoft.graph.specialFolder"
  },
  "video": {
    "@odata.type": "microsoft.graph.video",
    "audioBitsPerSample": 2,
    "audioChannels": 13,
    "audioFormat": "Audio Format value",
    "audioSamplesPerSecond": 5,
    "bitrate": 7,
    "fourCC": "Four CC value",
    "frameRate": "Double"
  },
  "webDavUrl": "https://example.com/webDavUrl/"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveitem"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.driveItem",
  "id": "6ae211ef-11ef-6ae2-ef11-e26aef11e26a",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "createdDateTime": "2016-12-31T23:57:35.7108579+03:00",
  "description": "Description value",
  "eTag": "ETag value",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "2016-12-31T23:58:38.9820934+03:00",
  "name": "Name value",
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference",
    "driveId": "Drive Id value",
    "driveType": "Drive Type value",
    "path": "Path value",
    "shareId": "Share Id value",
    "sharepointIds": {
      "@odata.type": "microsoft.graph.sharepointIds",
      "listId": "List Id value",
      "listItemId": "List Item Id value",
      "listItemUniqueId": "List Item Unique Id value",
      "siteId": "Site Id value",
      "siteUrl": "https://example.com/siteUrl/",
      "tenantId": "Tenant Id value",
      "webId": "Web Id value"
    }
  },
  "webUrl": "https://example.com/webUrl/",
  "audio": {
    "@odata.type": "microsoft.graph.audio",
    "album": "Album value",
    "albumArtist": "Album Artist value",
    "artist": "Artist value",
    "bitrate": 7,
    "composers": "Composers value",
    "copyright": "Copyright value",
    "disc": 4,
    "discCount": 9,
    "duration": 8,
    "genre": "Genre value",
    "hasDrm": true,
    "isVariableBitrate": true,
    "title": "Title value",
    "track": 5,
    "trackCount": 10,
    "year": 4
  },
  "bundle": {
    "@odata.type": "microsoft.graph.bundle",
    "childCount": 10,
    "album": {
      "@odata.type": "microsoft.graph.album",
      "coverImageItemId": "Cover Image Item Id value"
    }
  },
  "content": "Stream",
  "cTag": "CTag value",
  "deleted": {
    "@odata.type": "microsoft.graph.deleted",
    "state": "State value"
  },
  "file": {
    "@odata.type": "microsoft.graph.file",
    "hashes": {
      "@odata.type": "microsoft.graph.hashes",
      "crc32Hash": "Crc32Hash value",
      "quickXorHash": "Quick Xor Hash value",
      "sha1Hash": "Sha1Hash value",
      "sha256Hash": "Sha256Hash value"
    },
    "mimeType": "Mime Type value",
    "processingMetadata": true
  },
  "fileSystemInfo": {
    "@odata.type": "microsoft.graph.fileSystemInfo",
    "lastAccessedDateTime": "2017-01-01T00:01:56.0899806+03:00"
  },
  "folder": {
    "@odata.type": "microsoft.graph.folder",
    "view": {
      "@odata.type": "microsoft.graph.folderView",
      "sortBy": "Sort By value",
      "sortOrder": "Sort Order value",
      "viewType": "View Type value"
    }
  },
  "image": {
    "@odata.type": "microsoft.graph.image",
    "height": 6,
    "width": 5
  },
  "location": {
    "@odata.type": "microsoft.graph.geoCoordinates",
    "altitude": "Double",
    "latitude": "Double",
    "longitude": "Double"
  },
  "package": {
    "@odata.type": "microsoft.graph.package",
    "type": "Type value"
  },
  "pendingOperations": {
    "@odata.type": "microsoft.graph.pendingOperations",
    "pendingContentUpdate": {
      "@odata.type": "microsoft.graph.pendingContentUpdate",
      "queuedDateTime": "2016-12-31T23:59:00.2417573+03:00"
    }
  },
  "photo": {
    "@odata.type": "microsoft.graph.photo",
    "cameraMake": "Camera Make value",
    "cameraModel": "Camera Model value",
    "exposureDenominator": "Double",
    "exposureNumerator": "Double",
    "fNumber": "Double",
    "focalLength": "Double",
    "iso": 3,
    "orientation": 11,
    "takenDateTime": "2016-12-31T23:58:34.3648434+03:00"
  },
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet",
    "level": "Level value",
    "versionId": "Version Id value"
  },
  "remoteItem": {
    "@odata.type": "microsoft.graph.remoteItem",
    "shared": {
      "@odata.type": "microsoft.graph.shared",
      "owner": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "scope": "Scope value",
      "sharedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "sharedDateTime": "2016-12-31T23:59:32.0800584+03:00"
    },
    "size": 4,
    "specialFolder": {
      "@odata.type": "microsoft.graph.specialFolder"
    },
    "webDavUrl": "https://example.com/webDavUrl/"
  },
  "root": {
    "@odata.type": "microsoft.graph.root"
  },
  "searchResult": {
    "@odata.type": "microsoft.graph.searchResult",
    "onClickTelemetryUrl": "https://example.com/onClickTelemetryUrl/"
  },
  "shared": {
    "@odata.type": "microsoft.graph.shared"
  },
  "sharepointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "size": 4,
  "specialFolder": {
    "@odata.type": "microsoft.graph.specialFolder"
  },
  "video": {
    "@odata.type": "microsoft.graph.video",
    "audioBitsPerSample": 2,
    "audioChannels": 13,
    "audioFormat": "Audio Format value",
    "audioSamplesPerSecond": 5,
    "bitrate": 7,
    "fourCC": "Four CC value",
    "frameRate": "Double"
  },
  "webDavUrl": "https://example.com/webDavUrl/"
}
```

