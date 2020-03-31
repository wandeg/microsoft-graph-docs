---
title: "remove"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# remove

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
POST /sites/remove
POST /sites/{sitesId}/sites/remove
POST /groups/{groupsId}/sites/remove
POST /me/joinedGroups/{groupId}/sites/remove
POST /me/joinedGroups/{groupId}/sites/{siteId}/sites/remove
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
|value|[site](../resources/site.md) collection||



## Response
If successful, this action returns a `200 OK` response code and a [site](../resources/site.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "site_remove"
}
-->
``` http
POST https://graph.microsoft.com/beta/sites/remove

Content-type: application/json
Content-length: 990

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.site",
      "id": "6b6d9e06-9e06-6b6d-069e-6d6b069e6d6b",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
      "description": "Description value",
      "eTag": "ETag value",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00",
      "name": "Name value",
      "parentReference": {
        "@odata.type": "microsoft.graph.itemReference"
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
        "@odata.type": "microsoft.graph.siteCollection"
      }
    }
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.site)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 990

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.site",
      "id": "6b6d9e06-9e06-6b6d-069e-6d6b069e6d6b",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
      "description": "Description value",
      "eTag": "ETag value",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00",
      "name": "Name value",
      "parentReference": {
        "@odata.type": "microsoft.graph.itemReference"
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
        "@odata.type": "microsoft.graph.siteCollection"
      }
    }
  ]
}
```

