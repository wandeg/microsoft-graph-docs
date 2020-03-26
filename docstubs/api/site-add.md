---
title: "add"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# add

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
POST /sites/add
POST /sites/{sitesId}/sites/add
POST /groups/{groupsId}/sites/add
POST /me/joinedGroups/{groupId}/sites/add
POST /me/joinedGroups/{groupId}/sites/{siteId}/sites/add
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
  "name": "site_add"
}
-->
``` http
POST https://graph.microsoft.com/beta/sites/add

Content-type: application/json
Content-length: 991

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.site",
      "id": "3f2bb4eb-b4eb-3f2b-ebb4-2b3febb42b3f",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "createdDateTime": "2016-12-31T23:59:31.6288943+00:00",
      "description": "Description value",
      "eTag": "ETag value",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "2017-01-01T00:01:43.6555924+00:00",
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
Content-Length: 991

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.site",
      "id": "3f2bb4eb-b4eb-3f2b-ebb4-2b3febb42b3f",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "createdDateTime": "2016-12-31T23:59:31.6288943+00:00",
      "description": "Description value",
      "eTag": "ETag value",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "2017-01-01T00:01:43.6555924+00:00",
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

