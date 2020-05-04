---
title: "Get teamsCatalogApp"
description: "Read properties and relationships of a teamsCatalogApp object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get teamsCatalogApp

Namespace: microsoft.graph

Read properties and relationships of a [teamsCatalogApp](../resources/teamscatalogapp.md) object.

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
GET /teams/{teamsId}/apps/{teamsCatalogAppId}
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/apps/{teamsCatalogAppId}
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
If successful, this method returns a `200 OK` response code and a [teamsCatalogApp](../resources/teamscatalogapp.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_teamscatalogapp"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/apps/{teamsCatalogAppId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsCatalogApp"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.teamsCatalogApp",
    "id": "d0a20ea2-0ea2-d0a2-a20e-a2d0a20ea2d0",
    "externalId": "External Id value",
    "name": "Name value",
    "distributionMethod": "String"
  }
}
```

