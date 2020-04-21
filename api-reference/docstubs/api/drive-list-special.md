---
title: "List special"
description: "Get the driveItems from the special navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List special

Namespace: microsoft.graph

Get the driveItems from the special navigation property.

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
GET /drive/special
GET /drives/{drivesId}/special
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [driveItem](../resources/driveitem.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_driveitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/drive/special
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.driveitem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.driveItem",
      "id": "31696bd0-6bd0-3169-d06b-6931d06b6931",
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
      "createdDateTime": "2017-01-01T00:01:28.5453509+00:00",
      "description": "Description value",
      "eTag": "ETag value",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "2017-01-01T00:01:26.0388723+00:00",
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
        "lastAccessedDateTime": "2016-12-31T23:58:24.6598438+00:00"
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
        "takenDateTime": "2016-12-31T23:58:25.1048998+00:00"
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
          "sharedDateTime": "2016-12-31T23:59:21.0108234+00:00"
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
  ]
}
```

