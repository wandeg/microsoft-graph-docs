---
title: "Delete driveItem"
description: "Deletes a driveItem."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Delete driveItem

Namespace: microsoft.graph

Deletes a [driveItem](../resources/driveitem.md).

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
DELETE /drives/{drivesId}/root
DELETE /shares/{sharesId}/root
DELETE /workbooks/{workbooksId}
DELETE /shares/{sharesId}/driveItem
DELETE /me/joinedGroups/{groupId}/drive/root
DELETE /drives/{drivesId}/items/{driveItemId}
DELETE /shares/{sharesId}/items/{driveItemId}
DELETE /drives/{drivesId}/bundles/{driveItemId}
DELETE /drives/{drivesId}/special/{driveItemId}
DELETE /drives/{drivesId}/following/{driveItemId}
DELETE /workbooks/{workbooksId}/children/{driveItemId}
DELETE /me/joinedGroups/{groupId}/drive/items/{driveItemId}
DELETE /me/joinedGroups/{groupId}/drive/bundles/{driveItemId}
DELETE /me/joinedGroups/{groupId}/drive/special/{driveItemId}
DELETE /me/joinedGroups/{groupId}/drive/following/{driveItemId}
DELETE /me/joinedGroups/{groupId}/team/channels/{channelId}/filesFolder
DELETE /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem
DELETE /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/listItem/driveItem
DELETE /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/children/{driveItemId}
DELETE /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/root
DELETE /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/driveItem
DELETE /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/items/{driveItemId}
DELETE /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/analytics/itemActivityStats/{itemActivityStatId}/activities/{itemActivityId}/driveItem
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `204 No Content` response code.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "delete_driveitem"
}
-->
``` http
DELETE https://graph.microsoft.com/localtest/drives/{drivesId}/root
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

