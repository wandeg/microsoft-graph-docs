---
title: "driveItem: invite"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# invite

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
POST /drive/root/invite
POST /drives/{drivesId}/root/invite
POST /shares/{sharesId}/root/invite
POST /workbooks/{workbooksId}/invite
POST /drive/items/{driveItemId}/invite
POST /shares/{sharesId}/driveItem/invite
POST /drive/bundles/{driveItemId}/invite
POST /drive/special/{driveItemId}/invite
POST /drive/following/{driveItemId}/invite
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
|requireSignIn|Boolean|**TODO: Add Description**|
|roles|String collection|**TODO: Add Description**|
|sendInvitation|Boolean|**TODO: Add Description**|
|message|String|**TODO: Add Description**|
|recipients|[driveRecipient](../resources/driverecipient.md) collection|**TODO: Add Description**|
|expirationDateTime|String|**TODO: Add Description**|
|password|String|**TODO: Add Description**|



## Response
If successful, this action returns a `200 OK` response code and a [permission](../resources/permission.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "driveitem_invite"
}
-->
``` http
POST https://graph.microsoft.com/beta/drive/root/invite

Content-Type: application/json
Content-length: 308

{
  "requireSignIn": true,
  "roles": [
    "Roles value"
  ],
  "sendInvitation": true,
  "message": "Message value",
  "recipients": [
    {
      "@odata.type": "microsoft.graph.driveRecipient"
    }
  ],
  "expirationDateTime": "Expiration Date Time value",
  "password": "Password value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.permission)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.permission",
      "id": "aa6c0867-0867-aa6c-6708-6caa67086caa",
      "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
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

