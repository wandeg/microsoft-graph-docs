---
title: "getByPath"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getByPath



## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /sites/{sitesId}/getByPath
GET /shares/{sharesId}/site/getByPath
GET /sites/{sitesId}/sites/{siteId}/getByPath
GET /groups/{groupsId}/sites/{siteId}/getByPath
GET /me/joinedTeams/{groupId}/sites/{siteId}/getByPath
GET /me/joinedTeams/{groupId}/sites/{siteId}/sites/{siteId}/getByPath
GET /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/site/getByPath
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|path|String||



## Response
If successful, this function returns a `200 OK` response code and a [site](../resources/site.md) in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "site_getbypath"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/sites/{sitesId}/getByPath(path='parameterValue')
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
Content-Length: 923

{
  "value": {
    "@odata.type": "#microsoft.graph.site",
    "id": "6e6e652c-652c-6e6e-2c65-6e6e2c656e6e",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "createdDateTime": "2016-12-31T23:57:22.3554145+03:00",
    "description": "Description value",
    "eTag": "ETag value",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "2016-12-31T23:59:09.8413999+03:00",
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
}
```

