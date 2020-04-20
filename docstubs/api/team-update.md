---
title: "Update team"
description: "Update the properties of a team object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update team

Namespace: microsoft.graph

Update the properties of a [team](../resources/team.md) object.

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
PATCH /teams/{teamsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [team](../resources/team.md) object.

The following table shows the properties that are required when you create the [team](../resources/team.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|internalId|String|**TODO: Add Description**|
|classification|String|**TODO: Add Description**|
|specialization|teamSpecialization|**TODO: Add Description**. Possible values are: `none`, `educationStandard`, `educationClass`, `educationProfessionalLearningCommunity`, `educationStaff`, `healthcareStandard`, `healthcareCareCoordination`, `unknownFutureValue`.|
|visibility|teamVisibilityType|**TODO: Add Description**. Possible values are: `private`, `public`, `hiddenMembership`, `unknownFutureValue`.|
|webUrl|String|**TODO: Add Description**|
|memberSettings|[teamMemberSettings](../resources/teammembersettings.md)|**TODO: Add Description**|
|guestSettings|[teamGuestSettings](../resources/teamguestsettings.md)|**TODO: Add Description**|
|messagingSettings|[teamMessagingSettings](../resources/teammessagingsettings.md)|**TODO: Add Description**|
|funSettings|[teamFunSettings](../resources/teamfunsettings.md)|**TODO: Add Description**|
|discoverySettings|[teamDiscoverySettings](../resources/teamdiscoverysettings.md)|**TODO: Add Description**|
|isArchived|Boolean|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [team](../resources/team.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_team"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teams/{teamsId}
Content-Type: application/json
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.team",
  "id": "e9727aa7-7aa7-e972-a77a-72e9a77a72e9",
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

