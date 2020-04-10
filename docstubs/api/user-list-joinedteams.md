---
title: "List joinedTeams"
description: "Get the teams from the joinedTeams navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List joinedTeams

Namespace: microsoft.graph

Get the teams from the joinedTeams navigation property.

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
GET /me/joinedTeams
GET /users/{usersId}/joinedTeams
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
If successful, this method returns a `200 OK` response code and a collection of [team](../resources/team.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_team"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedTeams
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.team)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1606

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.team",
      "id": "21ace052-e052-21ac-52e0-ac2152e0ac21",
      "displayName": "Display Name value",
      "description": "Description value",
      "internalId": "Internal Id value",
      "classification": "Classification value",
      "specialization": "String",
      "visibility": "String",
      "webUrl": "https://example.com/webUrl/",
      "memberSettings": {
        "@odata.type": "microsoft.graph.teamMemberSettings",
        "allowCreateUpdateChannels": true,
        "allowCreatePrivateChannels": true,
        "allowDeleteChannels": true,
        "allowAddRemoveApps": true,
        "allowCreateUpdateRemoveTabs": true,
        "allowCreateUpdateRemoveConnectors": true
      },
      "guestSettings": {
        "@odata.type": "microsoft.graph.teamGuestSettings"
      },
      "messagingSettings": {
        "@odata.type": "microsoft.graph.teamMessagingSettings",
        "allowUserEditMessages": true,
        "allowUserDeleteMessages": true,
        "allowOwnerDeleteMessages": true,
        "allowTeamMentions": true,
        "allowChannelMentions": true
      },
      "funSettings": {
        "@odata.type": "microsoft.graph.teamFunSettings",
        "allowGiphy": true,
        "giphyContentRating": "String",
        "allowStickersAndMemes": true,
        "allowCustomMemes": true
      },
      "discoverySettings": {
        "@odata.type": "microsoft.graph.teamDiscoverySettings",
        "showInTeamsSearchAndSuggestions": true
      },
      "isArchived": true
    }
  ]
}
```

