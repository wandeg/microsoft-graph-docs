---
title: "driveItem: createLink"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# createLink

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
POST /drive/root/createLink
POST /drives/{drivesId}/root/createLink
POST /shares/{sharesId}/root/createLink
POST /workbooks/{workbooksId}/createLink
POST /drive/items/{driveItemId}/createLink
POST /shares/{sharesId}/driveItem/createLink
POST /drive/bundles/{driveItemId}/createLink
POST /drive/special/{driveItemId}/createLink
POST /drive/following/{driveItemId}/createLink
POST /drives/{drivesId}/items/{driveItemId}/createLink
POST /shares/{sharesId}/items/{driveItemId}/createLink
POST /drives/{drivesId}/bundles/{driveItemId}/createLink
POST /drives/{drivesId}/special/{driveItemId}/createLink
POST /drives/{drivesId}/following/{driveItemId}/createLink
POST /workbooks/{workbooksId}/children/{driveItemId}/createLink
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
|type|String|**TODO: Add Description**|
|scope|String|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|password|String|**TODO: Add Description**|
|message|String|**TODO: Add Description**|
|recipients|[driveRecipient](../resources/driverecipient.md) collection|**TODO: Add Description**|



## Response
If successful, this action returns a `200 OK` response code and a [permission](../resources/permission.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "driveitem_createlink"
}
-->
``` http
POST https://graph.microsoft.com/beta/drive/root/createLink

Content-Type: application/json
Content-length: 344

{
  "type": "Type value",
  "scope": "Scope value",
  "expirationDateTime": "2016-12-31T23:59:10.7331181+03:00",
  "password": "Password value",
  "message": "Message value",
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
  "@odata.type": "microsoft.graph.permission"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.permission",
    "id": "f7df381f-381f-f7df-1f38-dff71f38dff7",
    "expirationDateTime": "2016-12-31T23:59:10.7331181+03:00",
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
}
```

