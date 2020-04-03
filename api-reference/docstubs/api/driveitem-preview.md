---
title: "preview"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# preview

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
POST /drives/{drivesId}/root/preview
POST /shares/{sharesId}/root/preview
POST /workbooks/{workbooksId}/preview
POST /shares/{sharesId}/driveItem/preview
POST /me/joinedGroups/{groupId}/drive/root/preview
POST /drives/{drivesId}/items/{driveItemId}/preview
POST /shares/{sharesId}/items/{driveItemId}/preview
POST /drives/{drivesId}/bundles/{driveItemId}/preview
POST /drives/{drivesId}/special/{driveItemId}/preview
POST /drives/{drivesId}/following/{driveItemId}/preview
POST /workbooks/{workbooksId}/children/{driveItemId}/preview
POST /me/joinedGroups/{groupId}/drive/items/{driveItemId}/preview
POST /me/joinedGroups/{groupId}/drive/bundles/{driveItemId}/preview
POST /me/joinedGroups/{groupId}/drive/special/{driveItemId}/preview
POST /me/joinedGroups/{groupId}/drive/following/{driveItemId}/preview
POST /me/joinedGroups/{groupId}/team/channels/{channelId}/filesFolder/preview
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/preview
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/listItem/driveItem/preview
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/children/{driveItemId}/preview
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/root/preview
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/driveItem/preview
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/items/{driveItemId}/preview
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/analytics/itemActivityStats/{itemActivityStatId}/activities/{itemActivityId}/driveItem/preview
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
|viewer|String||
|chromeless|Boolean||
|allowEdit|Boolean||
|page|String||
|zoom|Double||



## Response
If successful, this action returns a `200 OK` response code and a [itemPreviewInfo](../resources/itempreviewinfo.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "driveitem_preview"
}
-->
``` http
POST https://graph.microsoft.com/beta/drives/{drivesId}/root/preview

Content-type: application/json
Content-length: 123

{
  "viewer": "Viewer value",
  "chromeless": true,
  "allowEdit": true,
  "page": "Page value",
  "zoom": "Double"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itempreviewinfo"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 77

{
  "value": {
    "@odata.type": "microsoft.graph.itemPreviewInfo"
  }
}
```

