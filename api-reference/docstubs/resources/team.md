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


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List teams](../api/team-list.md)|[team](../resources/team.md) collection|Get a list of the [team](../resources/team.md) objects and their properties.|
|[Get team](../api/team-get.md)|[team](../resources/team.md)|Read the properties and relationships of a [team](../resources/team.md) object.|
|[Create team](../api/team-post-teams.md)|[team](../resources/team.md)|Create a new [team](../resources/team.md) object.|
|[Delete team](../api/team-delete.md)|None|Deletes a [team](../resources/team.md) object.|
|[Update team](../api/team-update.md)|[team](../resources/team.md)|Update the properties of a [team](../resources/team.md) object.|
|[clone](../api/team-clone.md)|None|**TODO: Add Description**|
|[archive](../api/team-archive.md)|None|**TODO: Add Description**|
|[unarchive](../api/team-unarchive.md)|None|**TODO: Add Description**|
|[allMessages](../api/team-allmessages.md)|[chatMessage](../resources/chatmessage.md) collection|**TODO: Add Description**|
|[List schedule](../api/team-list-schedule.md)|[schedule](../resources/schedule.md) collection|Get the schedules from the schedule navigation property.|
|[Create schedule](../api/team-post-schedule.md)|[schedule](../resources/schedule.md)|Create a new schedule object.|
|[Delete schedule](../api/team-delete-schedule.md)|None|Delete a [schedule](../resources/schedule.md) object.|
|[Update schedule](../api/team-update-schedule.md)|[schedule](../resources/schedule.md)|Update the properties of a schedule object.|
|[Get schedule](../api/schedule-get.md)|[schedule](../resources/schedule.md)|Read the properties and relationships of a [schedule](../resources/schedule.md) object.|
|[List group](../api/team-list-group.md)|[group](../resources/group.md) collection|Get the groups from the group navigation property.|
|[Add group](../api/team-post-group.md)|[group](../resources/group.md)|Add group by posting to the group collection.|
|[Remove group](../api/team-delete-group.md)|None|Remove a [group](../resources/group.md) object.|
|[List template](../api/team-list-template.md)|[teamsTemplate](../resources/teamstemplate.md) collection|Get the teamsTemplates from the template navigation property.|
|[Add template](../api/team-post-template.md)|[teamsTemplate](../resources/teamstemplate.md)|Add template by posting to the template collection.|
|[Remove template](../api/team-delete-template.md)|None|Remove a [teamsTemplate](../resources/teamstemplate.md) object.|
|[List photo](../api/team-list-photo.md)|[profilePhoto](../resources/profilephoto.md) collection|Get the profilePhotoes from the photo navigation property.|
|[Create photo](../api/team-post-photo.md)|[profilePhoto](../resources/profilephoto.md)|Create a new photo object.|
|[Delete photo](../api/team-delete-photo.md)|None|Delete a [profilePhoto](../resources/profilephoto.md) object.|
|[Update photo](../api/team-update-photo.md)|[profilePhoto](../resources/profilephoto.md)|Update the properties of a photo object.|
|[Get profilePhoto](../api/profilephoto-get.md)|[profilePhoto](../resources/profilephoto.md)|Read the properties and relationships of a [profilePhoto](../resources/profilephoto.md) object.|
|[List owners](../api/team-list-owners.md)|[user](../resources/user.md) collection|Get the users from the owners navigation property.|
|[Add owners](../api/team-post-owners.md)|[user](../resources/user.md)|Add owners by posting to the owners collection.|
|[Remove owners](../api/team-delete-owners.md)|None|Remove an [user](../resources/user.md) object.|
|[List channels](../api/team-list-channels.md)|[channel](../resources/channel.md) collection|Get the channels from the channels navigation property.|
|[Create channels](../api/team-post-channels.md)|[channel](../resources/channel.md)|Create a new channels object.|
|[Delete channels](../api/team-delete-channels.md)|None|Delete a [channel](../resources/channel.md) object.|
|[Update channels](../api/team-update-channels.md)|[channel](../resources/channel.md)|Update the properties of a channels object.|
|[Get channel](../api/channel-get.md)|[channel](../resources/channel.md)|Read the properties and relationships of a [channel](../resources/channel.md) object.|
|[List primaryChannel](../api/team-list-primarychannel.md)|[channel](../resources/channel.md) collection|Get the channels from the primaryChannel navigation property.|
|[Create primaryChannel](../api/team-post-primarychannel.md)|[channel](../resources/channel.md)|Create a new primaryChannel object.|
|[Delete primaryChannel](../api/team-delete-primarychannel.md)|None|Delete a [channel](../resources/channel.md) object.|
|[Update primaryChannel](../api/team-update-primarychannel.md)|[channel](../resources/channel.md)|Update the properties of a primaryChannel object.|
|[Get channel](../api/channel-get.md)|[channel](../resources/channel.md)|Read the properties and relationships of a [channel](../resources/channel.md) object.|
|[List apps](../api/team-list-apps.md)|[teamsCatalogApp](../resources/teamscatalogapp.md) collection|Get the teamsCatalogApps from the apps navigation property.|
|[Create apps](../api/team-post-apps.md)|[teamsCatalogApp](../resources/teamscatalogapp.md)|Create a new apps object.|
|[Delete apps](../api/team-delete-apps.md)|None|Delete an [teamsCatalogApp](../resources/teamscatalogapp.md) object.|
|[Update apps](../api/team-update-apps.md)|[teamsCatalogApp](../resources/teamscatalogapp.md)|Update the properties of an apps object.|
|[Get teamsCatalogApp](../api/teamscatalogapp-get.md)|[teamsCatalogApp](../resources/teamscatalogapp.md)|Read the properties and relationships of a [teamsCatalogApp](../resources/teamscatalogapp.md) object.|
|[List installedApps](../api/team-list-installedapps.md)|[teamsAppInstallation](../resources/teamsappinstallation.md) collection|Get the teamsAppInstallations from the installedApps navigation property.|
|[Create installedApps](../api/team-post-installedapps.md)|[teamsAppInstallation](../resources/teamsappinstallation.md)|Create a new installedApps object.|
|[Delete installedApps](../api/team-delete-installedapps.md)|None|Delete an [teamsAppInstallation](../resources/teamsappinstallation.md) object.|
|[Update installedApps](../api/team-update-installedapps.md)|[teamsAppInstallation](../resources/teamsappinstallation.md)|Update the properties of an installedApps object.|
|[Get teamsAppInstallation](../api/teamsappinstallation-get.md)|[teamsAppInstallation](../resources/teamsappinstallation.md)|Read the properties and relationships of a [teamsAppInstallation](../resources/teamsappinstallation.md) object.|
|[List operations](../api/team-list-operations.md)|[teamsAsyncOperation](../resources/teamsasyncoperation.md) collection|Get the teamsAsyncOperations from the operations navigation property.|
|[Create operations](../api/team-post-operations.md)|[teamsAsyncOperation](../resources/teamsasyncoperation.md)|Create a new operations object.|
|[Delete operations](../api/team-delete-operations.md)|None|Delete an [teamsAsyncOperation](../resources/teamsasyncoperation.md) object.|
|[Update operations](../api/team-update-operations.md)|[teamsAsyncOperation](../resources/teamsasyncoperation.md)|Update the properties of an operations object.|
|[Get teamsAsyncOperation](../api/teamsasyncoperation-get.md)|[teamsAsyncOperation](../resources/teamsasyncoperation.md)|Read the properties and relationships of a [teamsAsyncOperation](../resources/teamsasyncoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|classification|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|discoverySettings|[teamDiscoverySettings](../resources/teamdiscoverysettings.md)|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|funSettings|[teamFunSettings](../resources/teamfunsettings.md)|**TODO: Add Description**|
|guestSettings|[teamGuestSettings](../resources/teamguestsettings.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|internalId|String|**TODO: Add Description**|
|isArchived|Boolean|**TODO: Add Description**|
|memberSettings|[teamMemberSettings](../resources/teammembersettings.md)|**TODO: Add Description**|
|messagingSettings|[teamMessagingSettings](../resources/teammessagingsettings.md)|**TODO: Add Description**|
|specialization|teamSpecialization|**TODO: Add Description**. Possible values are: `none`, `educationStandard`, `educationClass`, `educationProfessionalLearningCommunity`, `educationStaff`, `healthcareStandard`, `healthcareCareCoordination`, `unknownFutureValue`.|
|visibility|teamVisibilityType|**TODO: Add Description**. Possible values are: `private`, `public`, `hiddenMembership`, `unknownFutureValue`.|
|webUrl|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|apps|[teamsCatalogApp](../resources/teamscatalogapp.md) collection|**TODO: Add Description**|
|channels|[channel](../resources/channel.md) collection|**TODO: Add Description**|
|group|[group](../resources/group.md)|**TODO: Add Description**|
|installedApps|[teamsAppInstallation](../resources/teamsappinstallation.md) collection|**TODO: Add Description**|
|operations|[teamsAsyncOperation](../resources/teamsasyncoperation.md) collection|**TODO: Add Description**|
|owners|[user](../resources/user.md) collection|**TODO: Add Description**|
|photo|[profilePhoto](../resources/profilephoto.md)|**TODO: Add Description**|
|primaryChannel|[channel](../resources/channel.md)|**TODO: Add Description**|
|schedule|[schedule](../resources/schedule.md)|**TODO: Add Description**|
|template|[teamsTemplate](../resources/teamstemplate.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
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
  "displayName": "String",
  "description": "String",
  "internalId": "String",
  "classification": "String",
  "specialization": "String",
  "visibility": "String",
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
  "discoverySettings": {
    "@odata.type": "microsoft.graph.teamDiscoverySettings"
  },
  "isArchived": "Boolean"
}
```

