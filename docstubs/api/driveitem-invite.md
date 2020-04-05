---
title: "invite"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# invite

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
POST /me/drive/root/invite
POST /drives/{drivesId}/root/invite
POST /shares/{sharesId}/root/invite
POST /workbooks/{workbooksId}/invite
POST /shares/{sharesId}/driveItem/invite
POST /me/drive/items/{driveItemId}/invite
POST /me/drive/special/{driveItemId}/invite
POST /me/drive/following/{driveItemId}/invite
POST /drives/{drivesId}/items/{driveItemId}/invite
POST /shares/{sharesId}/items/{driveItemId}/invite
POST /drives/{drivesId}/special/{driveItemId}/invite
POST /drives/{drivesId}/following/{driveItemId}/invite
POST /workbooks/{workbooksId}/children/{driveItemId}/invite
POST /me/drive/following/{driveItemId}/listItem/driveItem/invite
POST /me/drive/following/{driveItemId}/children/{driveItemId}/invite
POST /me/followedSites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/root/invite
POST /me/followedSites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/driveItem/invite
POST /me/followedSites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/items/{driveItemId}/invite
POST /me/drive/following/{driveItemId}/analytics/itemActivityStats/{itemActivityStatId}/activities/{itemActivityId}/driveItem/invite
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
|requireSignIn|Boolean||
|roles|String collection||
|sendInvitation|Boolean||
|message|String||
|recipients|[driveRecipient](../resources/driverecipient.md) collection||
|expirationDateTime|String||
|password|String||



## Response
If successful, this action returns a `200 OK` response code and a [permission](../resources/permission.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "driveitem_invite"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/me/drive/root/invite

Content-type: application/json
Content-length: 377

{
  "requireSignIn": true,
  "roles": [
    "Roles value"
  ],
  "sendInvitation": true,
  "message": "Message value",
  "recipients": [
    {
      "@odata.type": "microsoft.graph.driveRecipient",
      "alias": "Alias value",
      "objectId": "Object Id value"
    }
  ],
  "expirationDateTime": "Expiration Date Time value",
  "password": "Password value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.permission)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 795

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.permission",
      "id": "14abd5c8-d5c8-14ab-c8d5-ab14c8d5ab14",
      "expirationDateTime": "2016-12-31T23:59:41.3794411+00:00",
      "grantedTo": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "grantedToIdentities": [
        {
          "@odata.type": "microsoft.graph.identitySet"
        }
      ],
      "hasPassword": true,
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
  ]
}
```

