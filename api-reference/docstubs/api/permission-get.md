---
title: "Get permission"
description: "Read the properties and relationships of a permission object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get permission

Namespace: microsoft.graph

Read the properties and relationships of a [permission](../resources/permission.md) object.

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
GET /workbooks/{workbooksId}/permissions/{permissionId}
GET /invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/permissions/{permissionId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [permission](../resources/permission.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_permission"
}
-->
``` http
GET https://graph.microsoft.com/beta/workbooks/{workbooksId}/permissions/{permissionId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
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
    "id": "405a5827-5827-405a-2758-5a4027585a40",
    "grantedTo": {
      "@odata.type": "microsoft.graph.identitySet",
      "application": {
        "@odata.type": "microsoft.graph.identity",
        "displayName": "Display Name value",
        "id": "Id value"
      },
      "device": {
        "@odata.type": "microsoft.graph.identity"
      },
      "user": {
        "@odata.type": "microsoft.graph.identity"
      }
    },
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
      "scope": "Scope value",
      "type": "Type value",
      "webUrl": "https://example.com/webUrl/"
    },
    "roles": [
      "Roles value"
    ],
    "shareId": "Share Id value"
  }
}
```

