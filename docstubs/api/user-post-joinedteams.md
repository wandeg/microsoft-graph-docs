---
title: "Add joinedTeams"
description: "Add joinedTeams by posting to the joinedTeams collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add joinedTeams

Namespace: microsoft.graph

Add joinedTeams by posting to the joinedTeams collection.

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
POST /me/joinedTeams/$ref
POST /users/{usersId}/joinedTeams/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [team](../resources/team.md) object.

The following table shows the properties that are required when you create the [team](../resources/team.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|internalId|String||
|classification|String||
|specialization|Enumeration| Possible values are: `none`, `educationStandard`, `educationClass`, `educationProfessionalLearningCommunity`, `educationStaff`, `healthcareStandard`, `healthcareCareCoordination`, `unknownFutureValue`.|
|visibility|Enumeration| Possible values are: `private`, `public`, `hiddenMembership`, `unknownFutureValue`.|
|webUrl|String||
|memberSettings|[teamMemberSettings](../resources/teammembersettings.md)||
|guestSettings|[teamGuestSettings](../resources/teamguestsettings.md)||
|messagingSettings|[teamMessagingSettings](../resources/teammessagingsettings.md)||
|funSettings|[teamFunSettings](../resources/teamfunsettings.md)||
|discoverySettings|[teamDiscoverySettings](../resources/teamdiscoverysettings.md)||
|isArchived|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [team](../resources/team.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_team_from_teams"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/joinedTeams
Content-type: application/json
Content-length: 1360

{
  "@odata.type": "#microsoft.graph.team",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1409

{
  "@odata.type": "#microsoft.graph.team",
  "id": "5bf2d2a3-d2a3-5bf2-a3d2-f25ba3d2f25b",
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
```

