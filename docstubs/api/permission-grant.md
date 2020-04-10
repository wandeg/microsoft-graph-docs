---
title: "permission: grant"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# grant

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
POST /shares/{sharesId}/permission/grant
POST /workbooks/{workbooksId}/permissions/{permissionId}/grant
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/permissions/{permissionId}/grant
POST /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/permission/grant
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
|roles|String collection||
|recipients|[driveRecipient](../resources/driverecipient.md) collection||



## Response
If successful, this action returns a `200 OK` response code and a [permission](../resources/permission.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "permission_grant"
}
-->
``` http
POST https://graph.microsoft.com/beta/shares/{sharesId}/permission/grant

Content-type: application/json
Content-length: 205

{
  "roles": [
    "Roles value"
  ],
  "recipients": [
    {
      "@odata.type": "microsoft.graph.driveRecipient",
      "alias": "Alias value",
      "objectId": "Object Id value"
    }
  ]
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
      "id": "8acfeec9-eec9-8acf-c9ee-cf8ac9eecf8a",
      "expirationDateTime": "2016-12-31T23:56:24.5775752+00:00",
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

