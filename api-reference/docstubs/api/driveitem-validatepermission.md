---
title: "validatePermission"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# validatePermission

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
POST /drives/{drivesId}/root/validatePermission
POST /shares/{sharesId}/root/validatePermission
POST /workbooks/{workbooksId}/validatePermission
POST /shares/{sharesId}/driveItem/validatePermission
POST /me/joinedGroups/{groupId}/drive/root/validatePermission
POST /drives/{drivesId}/items/{driveItemId}/validatePermission
POST /shares/{sharesId}/items/{driveItemId}/validatePermission
POST /drives/{drivesId}/bundles/{driveItemId}/validatePermission
POST /drives/{drivesId}/special/{driveItemId}/validatePermission
POST /drives/{drivesId}/following/{driveItemId}/validatePermission
POST /workbooks/{workbooksId}/children/{driveItemId}/validatePermission
POST /me/joinedGroups/{groupId}/drive/items/{driveItemId}/validatePermission
POST /me/joinedGroups/{groupId}/drive/bundles/{driveItemId}/validatePermission
POST /me/joinedGroups/{groupId}/drive/special/{driveItemId}/validatePermission
POST /me/joinedGroups/{groupId}/drive/following/{driveItemId}/validatePermission
POST /me/joinedGroups/{groupId}/team/channels/{channelId}/filesFolder/validatePermission
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/validatePermission
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/listItem/driveItem/validatePermission
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/children/{driveItemId}/validatePermission
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/root/validatePermission
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/driveItem/validatePermission
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/items/{driveItemId}/validatePermission
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/analytics/itemActivityStats/{itemActivityStatId}/activities/{itemActivityId}/driveItem/validatePermission
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
|challengeToken|String||
|password|String||



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "driveitem_validatepermission"
}
-->
``` http
POST https://graph.microsoft.com/beta/drives/{drivesId}/root/validatePermission

Content-type: application/json
Content-length: 82

{
  "challengeToken": "Challenge Token value",
  "password": "Password value"
}
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

