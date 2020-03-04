---
title: "createLink"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# createLink

Namespace: microsoft.graph



## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/drive/root/createLink
POST /drives/{drivesId}/root/createLink
POST /shares/{sharesId}/root/createLink
POST /workbooks/{workbooksId}/createLink
POST /shares/{sharesId}/driveItem/createLink
POST /me/drive/items/{driveItemId}/createLink
POST /me/drive/special/{driveItemId}/createLink
POST /drives/{drivesId}/items/{driveItemId}/createLink
POST /shares/{sharesId}/items/{driveItemId}/createLink
POST /drives/{drivesId}/special/{driveItemId}/createLink
POST /workbooks/{workbooksId}/children/{driveItemId}/createLink
POST /me/drive/items/{driveItemId}/listItem/driveItem/createLink
POST /me/drive/items/{driveItemId}/children/{driveItemId}/createLink
POST /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/root/createLink
POST /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/driveItem/createLink
POST /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/items/{driveItemId}/createLink
POST /me/drive/items/{driveItemId}/analytics/itemActivityStats/{itemActivityStatId}/activities/{itemActivityId}/driveItem/createLink
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|type|String||
|scope|String||



## Response
If successful, this action returns a `200 OK` response code and a [permission](../resources/permission.md) in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "driveitem_createlink"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/root/createLink

Content-type: application/json
Content-length: 55

{
  "type": "Type value",
  "scope": "Scope value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 531

{
  "value": {
    "@odata.type": "#microsoft.graph.permission",
    "id": "afa9fad8-fad8-afa9-d8fa-a9afd8faa9af",
    "grantedTo": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "inheritedFrom": {
      "@odata.type": "microsoft.graph.itemReference"
    },
    "invitation": {
      "@odata.type": "microsoft.graph.sharingInvitation"
    },
    "link": {
      "@odata.type": "microsoft.graph.sharingLink"
    },
    "roles": [
      "Roles value"
    ],
    "shareId": "Share Id value"
  }
}
```

