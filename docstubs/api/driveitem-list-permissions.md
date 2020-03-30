---
title: "List permissions"
description: "Get the permissions from the permissions navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List permissions

Namespace: microsoft.graph

Get the permissions from the permissions navigation property.

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
GET /workbooks/{workbooksId}/permissions
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/permissions
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [permission](../resources/permission.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_permission"
}
-->
``` http
GET https://graph.microsoft.com/beta/workbooks/{workbooksId}/permissions
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
Content-Length: 2183

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.permission",
      "id": "dce35389-5389-dce3-8953-e3dc8953e3dc",
      "expirationDateTime": "2016-12-31T23:57:00.3383939+03:00",
      "grantedTo": {
        "@odata.type": "microsoft.graph.identitySet",
        "application": {
          "@odata.type": "microsoft.graph.identity",
          "id": "Id value",
          "displayName": "Display Name value"
        },
        "device": {
          "@odata.type": "microsoft.graph.identity"
        },
        "user": {
          "@odata.type": "microsoft.graph.identity"
        }
      },
      "grantedToIdentities": [
        {
          "@odata.type": "microsoft.graph.identitySet"
        }
      ],
      "hasPassword": true,
      "inheritedFrom": {
        "@odata.type": "microsoft.graph.itemReference",
        "driveId": "Drive Id value",
        "driveType": "Drive Type value",
        "name": "Name value",
        "path": "Path value",
        "shareId": "Share Id value",
        "sharepointIds": {
          "@odata.type": "microsoft.graph.sharepointIds",
          "listId": "List Id value",
          "listItemId": "List Item Id value",
          "listItemUniqueId": "List Item Unique Id value",
          "siteId": "Site Id value",
          "siteUrl": "https://example.com/siteUrl/",
          "tenantId": "Tenant Id value",
          "webId": "Web Id value"
        }
      },
      "invitation": {
        "@odata.type": "microsoft.graph.sharingInvitation",
        "email": "Email value",
        "invitedBy": {
          "@odata.type": "microsoft.graph.identitySet"
        },
        "redeemedBy": "Redeemed By value",
        "signInRequired": true
      },
      "link": {
        "@odata.type": "microsoft.graph.sharingLink",
        "preventsDownload": true,
        "configuratorUrl": "https://example.com/configuratorUrl/",
        "scope": "Scope value",
        "type": "Type value",
        "webHtml": "Web Html value",
        "webUrl": "https://example.com/webUrl/"
      },
      "roles": [
        "Roles value"
      ],
      "shareId": "Share Id value"
    }
  ]
}
```

