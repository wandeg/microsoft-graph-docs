---
title: "Get team"
description: "Read properties and relationships of a team object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get team

Namespace: microsoft.graph

Read properties and relationships of a [team](../resources/team.md) object.

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
GET /teams/{teamsId}
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
If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_team"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.team",
    "id": "698a616b-616b-698a-6b61-8a696b618a69",
    "webUrl": "https://example.com/webUrl/",
    "memberSettings": {
      "@odata.type": "microsoft.graph.teamMemberSettings",
      "allowCreateUpdateChannels": true,
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
    "isArchived": true
  }
}
```

