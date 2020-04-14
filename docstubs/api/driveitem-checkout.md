---
title: "driveItem: checkout"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# checkout

Namespace: microsoft.graph



## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions. **|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /drives/{drivesId}/root/checkout
POST /shares/{sharesId}/root/checkout
POST /workbooks/{workbooksId}/checkout
POST /shares/{sharesId}/driveItem/checkout
POST /me/joinedGroups/{groupId}/drive/root/checkout
POST /drives/{drivesId}/items/{driveItemId}/checkout
POST /shares/{sharesId}/items/{driveItemId}/checkout
POST /drives/{drivesId}/bundles/{driveItemId}/checkout
POST /drives/{drivesId}/special/{driveItemId}/checkout
POST /drives/{drivesId}/following/{driveItemId}/checkout
POST /workbooks/{workbooksId}/children/{driveItemId}/checkout
POST /me/joinedGroups/{groupId}/drive/items/{driveItemId}/checkout
POST /me/joinedGroups/{groupId}/drive/bundles/{driveItemId}/checkout
POST /me/joinedGroups/{groupId}/drive/special/{driveItemId}/checkout
POST /me/joinedGroups/{groupId}/drive/following/{driveItemId}/checkout
POST /me/joinedGroups/{groupId}/team/channels/{channelId}/filesFolder/checkout
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/checkout
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/listItem/driveItem/checkout
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/children/{driveItemId}/checkout
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/root/checkout
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/driveItem/checkout
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/items/{driveItemId}/checkout
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/analytics/itemActivityStats/{itemActivityStatId}/activities/{itemActivityId}/driveItem/checkout
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
  "name": "driveitem_checkout"
}
-->
``` http
POST https://graph.microsoft.com/beta/drives/{drivesId}/root/checkout
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

