---
title: "List apps"
description: "Get the teamsCatalogApps from the apps navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List apps

Namespace: microsoft.graph

Get the teamsCatalogApps from the apps navigation property.

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
GET /teams/{teamsId}/apps
GET /me/joinedGroups/{groupId}/team/apps
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [teamsCatalogApp](../resources/teamscatalogapp.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_teamscatalogapp"
}
-->
``` http
GET https://graph.microsoft.com/localtest/teams/{teamsId}/apps
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.teamscatalogapp)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 257

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamsCatalogApp",
      "id": "11dd4ded-4ded-11dd-ed4d-dd11ed4ddd11",
      "externalId": "External Id value",
      "name": "Name value",
      "distributionMethod": "String"
    }
  ]
}
```

