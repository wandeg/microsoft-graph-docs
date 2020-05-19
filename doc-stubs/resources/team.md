---
title: "team resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# team resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List joinedTeams](../api/user-list-joinedteams.md)|[team](../resources/team.md) collection|Get the teams from the joinedTeams navigation property.|
|[Create joinedTeams](../api/user-post-joinedteams.md)|[team](../resources/team.md)|Create a new joinedTeams object.|
|[Delete joinedTeams](../api/user-delete-joinedteams.md)|None|Delete a [team](../resources/team.md) object.|
|[Update joinedTeams](../api/user-update-joinedteams.md)|[team](../resources/team.md)|Update the properties of a joinedTeams object.|
|[Get joinedTeams](../api/user-get-team.md)|[team](../resources/team.md)|Read the properties and relationships of a [team](../resources/team.md) object.|
|[List teams](../api/team-list.md)|[team](../resources/team.md) collection|Get a list of the [team](../resources/team.md) objects and their properties.|
|[Get team](../api/team-get.md)|[team](../resources/team.md)|Read the properties and relationships of a [team](../resources/team.md) object.|
|[Create team](../api/team-post-teams.md)|[team](../resources/team.md)|Create a new [team](../resources/team.md) object.|
|[Delete team](../api/team-delete.md)|None|Deletes a [team](../resources/team.md) object.|
|[Update team](../api/team-update.md)|[team](../resources/team.md)|Update the properties of a [team](../resources/team.md) object.|
|[clone](../api/team-clone.md)|None|**TODO: Add Description**|
|[archive](../api/team-archive.md)|None|**TODO: Add Description**|
|[unarchive](../api/team-unarchive.md)|None|**TODO: Add Description**|
|[List schedule](../api/team-list-schedule.md)|[schedule](../resources/schedule.md) collection|Get the schedules from the schedule navigation property.|
|[Create schedule](../api/team-post-schedule.md)|[schedule](../resources/schedule.md)|Create a new schedule object.|
|[Delete schedule](../api/team-delete-schedule.md)|None|Delete a [schedule](../resources/schedule.md) object.|
|[Update schedule](../api/team-update-schedule.md)|[schedule](../resources/schedule.md)|Update the properties of a schedule object.|
|[Get schedule](../api/team-get-schedule.md)|[schedule](../resources/schedule.md)|Read the properties and relationships of a [schedule](../resources/schedule.md) object.|
|[List channels](../api/team-list-channels.md)|[channel](../resources/channel.md) collection|Get the channels from the channels navigation property.|
|[Create channels](../api/team-post-channels.md)|[channel](../resources/channel.md)|Create a new channels object.|
|[Delete channels](../api/team-delete-channels.md)|None|Delete a [channel](../resources/channel.md) object.|
|[Update channels](../api/team-update-channels.md)|[channel](../resources/channel.md)|Update the properties of a channels object.|
|[Get channels](../api/team-get-channel.md)|[channel](../resources/channel.md)|Read the properties and relationships of a [channel](../resources/channel.md) object.|
|[List primaryChannel](../api/team-list-primarychannel.md)|[channel](../resources/channel.md) collection|Get the channels from the primaryChannel navigation property.|
|[Create primaryChannel](../api/team-post-primarychannel.md)|[channel](../resources/channel.md)|Create a new primaryChannel object.|
|[Delete primaryChannel](../api/team-delete-primarychannel.md)|None|Delete a [channel](../resources/channel.md) object.|
|[Update primaryChannel](../api/team-update-primarychannel.md)|[channel](../resources/channel.md)|Update the properties of a primaryChannel object.|
|[Get primaryChannel](../api/team-get-channel.md)|[channel](../resources/channel.md)|Read the properties and relationships of a [channel](../resources/channel.md) object.|
|[List installedApps](../api/team-list-installedapps.md)|[teamsAppInstallation](../resources/teamsappinstallation.md) collection|Get the teamsAppInstallations from the installedApps navigation property.|
|[Create installedApps](../api/team-post-installedapps.md)|[teamsAppInstallation](../resources/teamsappinstallation.md)|Create a new installedApps object.|
|[Delete installedApps](../api/team-delete-installedapps.md)|None|Delete a [teamsAppInstallation](../resources/teamsappinstallation.md) object.|
|[Update installedApps](../api/team-update-installedapps.md)|[teamsAppInstallation](../resources/teamsappinstallation.md)|Update the properties of an installedApps object.|
|[Get installedApps](../api/team-get-teamsappinstallation.md)|[teamsAppInstallation](../resources/teamsappinstallation.md)|Read the properties and relationships of a [teamsAppInstallation](../resources/teamsappinstallation.md) object.|
|[List operations](../api/team-list-operations.md)|[teamsAsyncOperation](../resources/teamsasyncoperation.md) collection|Get the teamsAsyncOperations from the operations navigation property.|
|[Create operations](../api/team-post-operations.md)|[teamsAsyncOperation](../resources/teamsasyncoperation.md)|Create a new operations object.|
|[Delete operations](../api/team-delete-operations.md)|None|Delete a [teamsAsyncOperation](../resources/teamsasyncoperation.md) object.|
|[Update operations](../api/team-update-operations.md)|[teamsAsyncOperation](../resources/teamsasyncoperation.md)|Update the properties of an operations object.|
|[Get operations](../api/team-get-teamsasyncoperation.md)|[teamsAsyncOperation](../resources/teamsasyncoperation.md)|Read the properties and relationships of a [teamsAsyncOperation](../resources/teamsasyncoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|funSettings|[teamFunSettings](../resources/teamfunsettings.md)|**TODO: Add Description**|
|guestSettings|[teamGuestSettings](../resources/teamguestsettings.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isArchived|Boolean|**TODO: Add Description**|
|memberSettings|[teamMemberSettings](../resources/teammembersettings.md)|**TODO: Add Description**|
|messagingSettings|[teamMessagingSettings](../resources/teammessagingsettings.md)|**TODO: Add Description**|
|webUrl|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|channels|[channel](../resources/channel.md) collection|**TODO: Add Description**|
|installedApps|[teamsAppInstallation](../resources/teamsappinstallation.md) collection|**TODO: Add Description**|
|operations|[teamsAsyncOperation](../resources/teamsasyncoperation.md) collection|**TODO: Add Description**|
|primaryChannel|[channel](../resources/channel.md)|**TODO: Add Description**|
|schedule|[schedule](../resources/schedule.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.team",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.team",
  "id": "String (identifier)",
  "webUrl": "String",
  "memberSettings": {
    "@odata.type": "microsoft.graph.teamMemberSettings"
  },
  "guestSettings": {
    "@odata.type": "microsoft.graph.teamGuestSettings"
  },
  "messagingSettings": {
    "@odata.type": "microsoft.graph.teamMessagingSettings"
  },
  "funSettings": {
    "@odata.type": "microsoft.graph.teamFunSettings"
  },
  "isArchived": "Boolean"
}
```

