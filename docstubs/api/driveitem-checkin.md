---
title: "driveItem: checkin"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# checkin

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
POST /drives/{drivesId}/root/checkin
POST /shares/{sharesId}/root/checkin
POST /workbooks/{workbooksId}/checkin
POST /shares/{sharesId}/driveItem/checkin
POST /me/joinedGroups/{groupId}/drive/root/checkin
POST /drives/{drivesId}/items/{driveItemId}/checkin
POST /shares/{sharesId}/items/{driveItemId}/checkin
POST /drives/{drivesId}/bundles/{driveItemId}/checkin
POST /drives/{drivesId}/special/{driveItemId}/checkin
POST /drives/{drivesId}/following/{driveItemId}/checkin
POST /workbooks/{workbooksId}/children/{driveItemId}/checkin
POST /me/joinedGroups/{groupId}/drive/items/{driveItemId}/checkin
POST /me/joinedGroups/{groupId}/drive/bundles/{driveItemId}/checkin
POST /me/joinedGroups/{groupId}/drive/special/{driveItemId}/checkin
POST /me/joinedGroups/{groupId}/drive/following/{driveItemId}/checkin
POST /me/joinedGroups/{groupId}/team/channels/{channelId}/filesFolder/checkin
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/checkin
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/listItem/driveItem/checkin
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/children/{driveItemId}/checkin
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/root/checkin
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/driveItem/checkin
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/items/{driveItemId}/checkin
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/analytics/itemActivityStats/{itemActivityStatId}/activities/{itemActivityId}/driveItem/checkin
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|checkInAs|String||
|comment|String||



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "driveitem_checkin"
}
-->
``` http
POST https://graph.microsoft.com/beta/drives/{drivesId}/root/checkin

Content-type: application/json
Content-length: 71

{
  "checkInAs": "Check In As value",
  "comment": "Comment value"
}
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

