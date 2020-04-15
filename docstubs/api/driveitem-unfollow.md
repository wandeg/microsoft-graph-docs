---
title: "driveItem: unfollow"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# unfollow

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
POST /drives/{drivesId}/root/unfollow
POST /shares/{sharesId}/root/unfollow
POST /workbooks/{workbooksId}/unfollow
POST /shares/{sharesId}/driveItem/unfollow
POST /me/joinedGroups/{groupId}/drive/root/unfollow
POST /drives/{drivesId}/items/{driveItemId}/unfollow
POST /shares/{sharesId}/items/{driveItemId}/unfollow
POST /drives/{drivesId}/bundles/{driveItemId}/unfollow
POST /drives/{drivesId}/special/{driveItemId}/unfollow
POST /drives/{drivesId}/following/{driveItemId}/unfollow
POST /workbooks/{workbooksId}/children/{driveItemId}/unfollow
POST /me/joinedGroups/{groupId}/drive/items/{driveItemId}/unfollow
POST /me/joinedGroups/{groupId}/drive/bundles/{driveItemId}/unfollow
POST /me/joinedGroups/{groupId}/drive/special/{driveItemId}/unfollow
POST /me/joinedGroups/{groupId}/drive/following/{driveItemId}/unfollow
POST /me/joinedGroups/{groupId}/team/channels/{channelId}/filesFolder/unfollow
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/unfollow
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/listItem/driveItem/unfollow
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/children/{driveItemId}/unfollow
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/root/unfollow
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/driveItem/unfollow
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/items/{driveItemId}/unfollow
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/analytics/itemActivityStats/{itemActivityStatId}/activities/{itemActivityId}/driveItem/unfollow
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "driveitem_unfollow"
}
-->
``` http
POST https://graph.microsoft.com/beta/drives/{drivesId}/root/unfollow
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

