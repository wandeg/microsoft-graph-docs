---
title: "Get teamsCatalogApp"
description: "Read properties and relationships of the teamsCatalogApp object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get teamsCatalogApp

Namespace: microsoft.graph

Read properties and relationships of the [teamsCatalogApp](../resources/teamscatalogapp.md) object.

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
GET /teams/{teamsId}/apps/{teamsCatalogAppId}
GET /me/joinedGroups/{groupId}/team/apps/{teamsCatalogAppId}
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
If successful, this method returns a `200 OK` response code and [teamsCatalogApp](../resources/teamscatalogapp.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_teamscatalogapp"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/apps/{teamsCatalogAppId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsCatalogApp"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "value": {
    "@odata.type": "#microsoft.graph.teamsCatalogApp",
    "id": "14ff47c5-47c5-14ff-c547-ff14c547ff14",
    "externalId": "External Id value",
    "name": "Name value",
    "distributionMethod": "String"
  }
}
```

