---
title: "driveItem: delta"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# delta

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /drives/{drivesId}/root/delta
GET /shares/{sharesId}/root/delta
GET /workbooks/{workbooksId}/delta
GET /shares/{sharesId}/driveItem/delta
GET /me/joinedGroups/{groupId}/drive/root/delta
GET /drives/{drivesId}/items/{driveItemId}/delta
GET /shares/{sharesId}/items/{driveItemId}/delta
GET /drives/{drivesId}/bundles/{driveItemId}/delta
GET /drives/{drivesId}/special/{driveItemId}/delta
GET /drives/{drivesId}/following/{driveItemId}/delta
GET /workbooks/{workbooksId}/children/{driveItemId}/delta
GET /me/joinedGroups/{groupId}/drive/items/{driveItemId}/delta
GET /me/joinedGroups/{groupId}/drive/bundles/{driveItemId}/delta
GET /me/joinedGroups/{groupId}/drive/special/{driveItemId}/delta
GET /me/joinedGroups/{groupId}/drive/following/{driveItemId}/delta
GET /me/joinedGroups/{groupId}/team/channels/{channelId}/filesFolder/delta
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/delta
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/listItem/driveItem/delta
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/children/{driveItemId}/delta
GET /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/root/delta
GET /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/driveItem/delta
GET /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/items/{driveItemId}/delta
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/analytics/itemActivityStats/{itemActivityStatId}/activities/{itemActivityId}/driveItem/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "driveitem_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/drives/{drivesId}/root/delta
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
      "id": "51ff9347-9347-51ff-4793-ff514793ff51",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "createdDateTime": "2016-12-31T23:56:51.3342982+03:00",
      "description": "Description value",
      "eTag": "ETag value",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "2016-12-31T23:56:35.1491722+03:00",
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

