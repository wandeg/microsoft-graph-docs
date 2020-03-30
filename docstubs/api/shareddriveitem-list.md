---
title: "List sharedDriveItems"
description: "List properties and relationships of the sharedDriveItem objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List sharedDriveItems

Namespace: microsoft.graph

List properties and relationships of the [sharedDriveItem](../resources/shareddriveitem.md) objects.

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
GET /shares
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
If successful, this method returns a `200 OK` response code and a collection of [sharedDriveItem](../resources/shareddriveitem.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_shareddriveitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/shares
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.shareddriveitem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1680

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sharedDriveItem",
      "id": "31e5e81b-e81b-31e5-1be8-e5311be8e531",
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
      "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
      "description": "Description value",
      "eTag": "ETag value",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
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
      "owner": {
        "@odata.type": "microsoft.graph.identitySet"
      }
    }
  ]
}
```

