---
title: "Get contentType"
description: "Read the properties and relationships of a contentType object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get contentType

Namespace: microsoft.graph

Read the properties and relationships of a [contentType](../resources/contenttype.md) object.

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
GET /sites/{sitesId}/contentTypes/{contentTypeId}
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/list/contentTypes/{contentTypeId}
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/sites/{siteId}/contentTypes/{contentTypeId}
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
If successful, this method returns a `200 OK` response code and a [contentType](../resources/contenttype.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_contenttype"
}
-->
``` http
GET https://graph.microsoft.com/beta/sites/{sitesId}/contentTypes/{contentTypeId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.contentType",
    "id": "c9f5d440-d440-c9f5-40d4-f5c940d4f5c9",
    "description": "Description value",
    "group": "Group value",
    "hidden": true,
    "inheritedFrom": {
      "@odata.type": "microsoft.graph.itemReference",
      "driveId": "Drive Id value",
      "driveType": "Drive Type value",
      "id": "Id value",
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
    "name": "Name value",
    "order": {
      "@odata.type": "microsoft.graph.contentTypeOrder",
      "default": true,
      "position": 8
    },
    "parentId": "Parent Id value",
    "readOnly": true,
    "sealed": true
  }
}
```

