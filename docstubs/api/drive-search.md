---
title: "search"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# search

Namespace: microsoft.graph



## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /drive/search
GET /me/drive/search
GET /drives/{drivesId}/search
GET /me/drives/{driveId}/search
GET /users/{usersId}/drive/search
GET /sites/{sitesId}/drive/search
GET /groups/{groupsId}/drive/search
GET /me/joinedGroups/{groupId}/drive/search
GET /users/{usersId}/drives/{driveId}/search
GET /sites/{sitesId}/drives/{driveId}/search
GET /groups/{groupsId}/drives/{driveId}/search
GET /me/joinedGroups/{groupId}/drive/list/drive/search
GET /me/joinedGroups/{groupId}/drives/{driveId}/search
GET /me/joinedGroups/{groupId}/sites/{siteId}/drive/search
GET /me/joinedGroups/{groupId}/sites/{siteId}/drives/{driveId}/search
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|q|String||



## Response
If successful, this function returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "drive_search"
}
-->
``` http
GET https://graph.microsoft.com/beta/drive/search(q='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.driveitem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2402

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.driveItem",
      "id": "9d3622d9-22d9-9d36-d922-369dd922369d",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
      "description": "Description value",
      "eTag": "ETag value",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
      "name": "Name value",
      "parentReference": {
        "@odata.type": "microsoft.graph.itemReference"
      },
      "webUrl": "https://example.com/webUrl/",
      "audio": {
        "@odata.type": "microsoft.graph.audio"
      },
      "bundle": {
        "@odata.type": "microsoft.graph.bundle"
      },
      "content": "Stream",
      "cTag": "CTag value",
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
      "size": 4,
      "specialFolder": {
        "@odata.type": "microsoft.graph.specialFolder"
      },
      "video": {
        "@odata.type": "microsoft.graph.video"
      },
      "webDavUrl": "https://example.com/webDavUrl/"
    }
  ]
}
```

