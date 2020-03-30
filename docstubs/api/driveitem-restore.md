---
title: "restore"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# restore

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
POST /drives/{drivesId}/root/restore
POST /shares/{sharesId}/root/restore
POST /workbooks/{workbooksId}/restore
POST /shares/{sharesId}/driveItem/restore
POST /me/joinedGroups/{groupId}/drive/root/restore
POST /drives/{drivesId}/items/{driveItemId}/restore
POST /shares/{sharesId}/items/{driveItemId}/restore
POST /drives/{drivesId}/bundles/{driveItemId}/restore
POST /drives/{drivesId}/special/{driveItemId}/restore
POST /drives/{drivesId}/following/{driveItemId}/restore
POST /workbooks/{workbooksId}/children/{driveItemId}/restore
POST /me/joinedGroups/{groupId}/drive/items/{driveItemId}/restore
POST /me/joinedGroups/{groupId}/drive/bundles/{driveItemId}/restore
POST /me/joinedGroups/{groupId}/drive/special/{driveItemId}/restore
POST /me/joinedGroups/{groupId}/drive/following/{driveItemId}/restore
POST /me/joinedGroups/{groupId}/team/channels/{channelId}/filesFolder/restore
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/restore
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/listItem/driveItem/restore
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/children/{driveItemId}/restore
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/root/restore
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/driveItem/restore
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/items/{driveItemId}/restore
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/analytics/itemActivityStats/{itemActivityStatId}/activities/{itemActivityId}/driveItem/restore
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|parentReference|[itemReference](../resources/itemreference.md)||
|name|String||



## Response
If successful, this action returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "driveitem_restore"
}
-->
``` http
POST https://graph.microsoft.com/beta/drives/{drivesId}/root/restore

Content-type: application/json
Content-length: 110

{
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference"
  },
  "name": "Name value"
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
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2232

{
  "value": {
    "@odata.type": "#microsoft.graph.driveItem",
    "id": "dccb3b05-3b05-dccb-053b-cbdc053bcbdc",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "createdDateTime": "2017-01-01T00:01:44.2536508+00:00",
    "description": "Description value",
    "eTag": "ETag value",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00",
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

