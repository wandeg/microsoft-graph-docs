---
title: "Get site"
description: "Read properties and relationships of the site object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get site

Namespace: microsoft.graph

Read properties and relationships of the [site](../resources/site.md) object.

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
GET /sites/{sitesId}
GET /shares/{sharesId}/site
GET /sites/{sitesId}/sites/{siteId}
GET /groups/{groupsId}/sites/{siteId}
GET /me/joinedGroups/{groupId}/sites/{siteId}
GET /me/joinedGroups/{groupId}/sites/{siteId}/sites/{siteId}
GET /me/joinedGroups/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/site
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
If successful, this method returns a `200 OK` response code and [site](../resources/site.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_site"
}
-->
``` http
GET https://graph.microsoft.com/beta/sites/{sitesId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.site"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1865

{
  "value": {
    "@odata.type": "#microsoft.graph.site",
    "id": "6a548c74-8c74-6a54-748c-546a748c546a",
    "createdBy": {
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
    "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
    "description": "Description value",
    "eTag": "ETag value",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
    "name": "Name value",
    "parentReference": {
      "@odata.type": "microsoft.graph.itemReference",
      "driveId": "Drive Id value",
      "driveType": "Drive Type value",
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
    "webUrl": "https://example.com/webUrl/",
    "displayName": "Display Name value",
    "root": {
      "@odata.type": "microsoft.graph.root"
    },
    "sharepointIds": {
      "@odata.type": "microsoft.graph.sharepointIds"
    },
    "siteCollection": {
      "@odata.type": "microsoft.graph.siteCollection",
      "dataLocationCode": "Data Location Code value",
      "hostname": "Hostname value"
    }
  }
}
```

