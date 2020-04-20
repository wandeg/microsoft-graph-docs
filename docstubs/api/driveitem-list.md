---
title: "List driveItems"
description: "Get a list of the driveItem objects and their properties."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List driveItems

Namespace: microsoft.graph

Get a list of the [driveItem](../resources/driveitem.md) objects and their properties.

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
GET /workbooks
GET /drive/items
GET /drive/bundles
GET /drive/special
GET /drive/following
GET /drives/{drivesId}/items
GET /shares/{sharesId}/items
GET /drives/{drivesId}/bundles
GET /drives/{drivesId}/special
GET /drives/{drivesId}/following
GET /workbooks/{workbooksId}/children
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
GET https://graph.microsoft.com/beta/workbooks
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
      "id": "7294cc0d-cc0d-7294-0dcc-94720dcc9472",
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
      "createdDateTime": "2016-12-31T23:57:02.5240758+03:00",
      "description": "Description value",
      "eTag": "ETag value",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "2017-01-01T00:01:44.3371159+03:00",
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
        "lastAccessedDateTime": "2017-01-01T00:03:20.5793144+03:00"
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
          "queuedDateTime": "2017-01-01T00:02:38.8900756+03:00"
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
        "takenDateTime": "2016-12-31T23:59:39.0623687+03:00"
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
          "sharedDateTime": "2016-12-31T23:58:02.856467+03:00"
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

