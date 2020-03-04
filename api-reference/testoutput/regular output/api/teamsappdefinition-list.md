---
title: "List teamsAppDefinitions"
description: "List properties and relationships of the teamsAppDefinition objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List teamsAppDefinitions

Namespace: microsoft.graph

List properties and relationships of the [teamsAppDefinition](../resources/teamsappdefinition.md) objects.

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
GET /me/joinedTeams/{groupId}/team/channels/{channelId}/tabs/{teamsTabId}/teamsApp/appDefinitions
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [teamsAppDefinition](../resources/teamsappdefinition.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_teamsappdefinition"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/joinedTeams/{groupId}/team/channels/{channelId}/tabs/{teamsTabId}/teamsApp/appDefinitions
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.teamsappdefinition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 272

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamsAppDefinition",
      "id": "2b2e69ba-69ba-2b2e-ba69-2e2bba692e2b",
      "teamsAppId": "Teams App Id value",
      "displayName": "Display Name value",
      "version": "Version value"
    }
  ]
}
```

