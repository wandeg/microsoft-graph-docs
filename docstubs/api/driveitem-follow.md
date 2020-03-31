---
title: "follow"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# follow

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
POST /drives/{drivesId}/root/follow
POST /shares/{sharesId}/root/follow
POST /workbooks/{workbooksId}/follow
POST /shares/{sharesId}/driveItem/follow
POST /me/joinedGroups/{groupId}/drive/root/follow
POST /drives/{drivesId}/items/{driveItemId}/follow
POST /shares/{sharesId}/items/{driveItemId}/follow
POST /drives/{drivesId}/bundles/{driveItemId}/follow
POST /drives/{drivesId}/special/{driveItemId}/follow
POST /drives/{drivesId}/following/{driveItemId}/follow
POST /workbooks/{workbooksId}/children/{driveItemId}/follow
POST /me/joinedGroups/{groupId}/drive/items/{driveItemId}/follow
POST /me/joinedGroups/{groupId}/drive/bundles/{driveItemId}/follow
POST /me/joinedGroups/{groupId}/drive/special/{driveItemId}/follow
POST /me/joinedGroups/{groupId}/drive/following/{driveItemId}/follow
POST /me/joinedGroups/{groupId}/team/channels/{channelId}/filesFolder/follow
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/follow
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/listItem/driveItem/follow
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/children/{driveItemId}/follow
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/root/follow
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/driveItem/follow
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/items/{driveItemId}/follow
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/analytics/itemActivityStats/{itemActivityStatId}/activities/{itemActivityId}/driveItem/follow
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this action returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "driveitem_follow"
}
-->
``` http
POST https://graph.microsoft.com/beta/drives/{drivesId}/root/follow
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
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2231

{
  "value": {
    "@odata.type": "#microsoft.graph.driveItem",
    "id": "8f6c26e2-26e2-8f6c-e226-6c8fe2266c8f",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "createdDateTime": "2016-12-31T23:58:10.4520456+03:00",
    "description": "Description value",
    "eTag": "ETag value",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "2017-01-01T00:02:23.471109+03:00",
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
}
```

