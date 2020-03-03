---
title: "Create driveItem"
description: "Create a new driveItem object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create driveItem

Create a new [driveItem](../resources/driveitem.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /workbooks
POST /me/drive/items
POST /me/drive/special
POST /drives/{drivesId}/items
POST /shares/{sharesId}/items
POST /drives/{drivesId}/special
POST /workbooks/{workbooksId}/children
POST /me/drive/items/{driveItemId}/children
POST /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/items
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the driveItem object.

The following table shows the properties that are required when you create the driveItem.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdBy|[identitySet](../resources/identitySet.md)| Inherited from [baseItem](../resources/baseItem.md)|
|createdDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseItem.md)|
|description|String| Inherited from [baseItem](../resources/baseItem.md)|
|eTag|String| Inherited from [baseItem](../resources/baseItem.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [baseItem](../resources/baseItem.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseItem.md)|
|name|String| Inherited from [baseItem](../resources/baseItem.md)|
|parentReference|[itemReference](../resources/itemReference.md)| Inherited from [baseItem](../resources/baseItem.md)|
|webUrl|String| Inherited from [baseItem](../resources/baseItem.md)|
|audio|[audio](../resources/audio.md)||
|content|Stream||
|cTag|String||
|deleted|[deleted](../resources/deleted.md)||
|file|[file](../resources/file.md)||
|fileSystemInfo|[fileSystemInfo](../resources/fileSystemInfo.md)||
|folder|[folder](../resources/folder.md)||
|image|[image](../resources/image.md)||
|location|[geoCoordinates](../resources/geoCoordinates.md)||
|package|[package](../resources/package.md)||
|photo|[photo](../resources/photo.md)||
|publication|[publicationFacet](../resources/publicationFacet.md)||
|remoteItem|[remoteItem](../resources/remoteItem.md)||
|root|[root](../resources/root.md)||
|searchResult|[searchResult](../resources/searchResult.md)||
|shared|[shared](../resources/shared.md)||
|sharepointIds|[sharepointIds](../resources/sharepointIds.md)||
|size|Int64||
|specialFolder|[specialFolder](../resources/specialFolder.md)||
|video|[video](../resources/video.md)||
|webDavUrl|String||



## Response
If successful, this method returns a `201 Created` response code and a [driveItem](../resources/driveitem.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_driveitem_from_workbooks"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/workbooks
Content-type: application/json
Content-length: 4666

{
  "@odata.type": "#microsoft.graph.driveItem",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "Display Name value",
      "id": "Id value"
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
      "sha1Hash": "Sha1Hash value"
    },
    "mimeType": "Mime Type value",
    "processingMetadata": true
  },
  "fileSystemInfo": {
    "@odata.type": "microsoft.graph.fileSystemInfo",
    "lastAccessedDateTime": "2017-01-01T00:03:08.8222757+03:00"
  },
  "folder": {
    "@odata.type": "microsoft.graph.folder",
    "childCount": 10,
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
  "photo": {
    "@odata.type": "microsoft.graph.photo",
    "cameraMake": "Camera Make value",
    "cameraModel": "Camera Model value",
    "exposureDenominator": "Double",
    "exposureNumerator": "Double",
    "fNumber": "Double",
    "focalLength": "Double",
    "iso": 3,
    "takenDateTime": "2017-01-01T00:02:52.7967897+03:00"
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
      "sharedDateTime": "2016-12-31T23:58:33.5002076+03:00"
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveitem"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4917

{
  "@odata.type": "#microsoft.graph.driveItem",
  "id": "ffa050b0-50b0-ffa0-b050-a0ffb050a0ff",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "Display Name value",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "createdDateTime": "2016-12-31T23:57:22.3554145+03:00",
  "description": "Description value",
  "eTag": "ETag value",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "2016-12-31T23:59:09.8413999+03:00",
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
      "sha1Hash": "Sha1Hash value"
    },
    "mimeType": "Mime Type value",
    "processingMetadata": true
  },
  "fileSystemInfo": {
    "@odata.type": "microsoft.graph.fileSystemInfo",
    "lastAccessedDateTime": "2017-01-01T00:03:08.8222757+03:00"
  },
  "folder": {
    "@odata.type": "microsoft.graph.folder",
    "childCount": 10,
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
  "photo": {
    "@odata.type": "microsoft.graph.photo",
    "cameraMake": "Camera Make value",
    "cameraModel": "Camera Model value",
    "exposureDenominator": "Double",
    "exposureNumerator": "Double",
    "fNumber": "Double",
    "focalLength": "Double",
    "iso": 3,
    "takenDateTime": "2017-01-01T00:02:52.7967897+03:00"
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
      "sharedDateTime": "2016-12-31T23:58:33.5002076+03:00"
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

