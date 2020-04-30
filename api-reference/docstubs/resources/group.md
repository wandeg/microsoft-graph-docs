---
title: "group resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# group resource type


Namespace: microsoft.graph

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List groups](../api/group-list.md)|[group](../resources/group.md) collection|Get a list of the [group](../resources/group.md) objects and their properties.|
|[Get group](../api/group-get.md)|[group](../resources/group.md)|Read the properties and relationships of a [group](../resources/group.md) object.|
|[Create group](../api/group-post-groups.md)|[group](../resources/group.md)|Create a new [group](../resources/group.md) object.|
|[Delete group](../api/group-delete.md)|None|Deletes a [group](../resources/group.md) object.|
|[Update group](../api/group-update.md)|[group](../resources/group.md)|Update the properties of a [group](../resources/group.md) object.|
|[delta](../api/group-delta.md)|[group](../resources/group.md) collection|**TODO: Add Description**|
|[evaluateDynamicMembership](../api/group-evaluatedynamicmembership.md)|[evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md)|**TODO: Add Description**|
|[checkMemberGroups](../api/group-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/group-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/group-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/group-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/group-restore.md)|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|[validateProperties](../api/group-validateproperties.md)|None|**TODO: Add Description**|
|[checkGrantedPermissionsForApp](../api/group-checkgrantedpermissionsforapp.md)|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) collection|**TODO: Add Description**|
|[assignLicense](../api/group-assignlicense.md)|[group](../resources/group.md)|**TODO: Add Description**|
|[subscribeByMail](../api/group-subscribebymail.md)|None|**TODO: Add Description**|
|[unsubscribeByMail](../api/group-unsubscribebymail.md)|None|**TODO: Add Description**|
|[addFavorite](../api/group-addfavorite.md)|None|**TODO: Add Description**|
|[removeFavorite](../api/group-removefavorite.md)|None|**TODO: Add Description**|
|[resetUnseenCount](../api/group-resetunseencount.md)|None|**TODO: Add Description**|
|[renew](../api/group-renew.md)|None|**TODO: Add Description**|
|[evaluateDynamicMembership](../api/group-evaluatedynamicmembership.md)|[evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md)|**TODO: Add Description**|
|[List appRoleAssignments](../api/group-list-approleassignments.md)|[appRoleAssignment](../resources/approleassignment.md) collection|Get the appRoleAssignments from the appRoleAssignments navigation property.|
|[Create appRoleAssignments](../api/group-post-approleassignments.md)|[appRoleAssignment](../resources/approleassignment.md)|Create a new appRoleAssignments object.|
|[Delete appRoleAssignments](../api/group-delete-approleassignments.md)|None|Delete an [appRoleAssignment](../resources/approleassignment.md) object.|
|[Update appRoleAssignments](../api/group-update-approleassignments.md)|[appRoleAssignment](../resources/approleassignment.md)|Update the properties of an appRoleAssignments object.|
|[Get appRoleAssignment](../api/approleassignment-get.md)|[appRoleAssignment](../resources/approleassignment.md)|Read the properties and relationships of an [appRoleAssignment](../resources/approleassignment.md) object.|
|[List members](../api/group-list-members.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the members navigation property.|
|[Add members](../api/group-post-members.md)|[directoryObject](../resources/directoryobject.md)|Add members by posting to the members collection.|
|[Remove members](../api/group-delete-members.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List membersWithLicenseErrors](../api/group-list-memberswithlicenseerrors.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the membersWithLicenseErrors navigation property.|
|[Add membersWithLicenseErrors](../api/group-post-memberswithlicenseerrors.md)|[directoryObject](../resources/directoryobject.md)|Add membersWithLicenseErrors by posting to the membersWithLicenseErrors collection.|
|[Remove membersWithLicenseErrors](../api/group-delete-memberswithlicenseerrors.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List memberOf](../api/group-list-memberof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the memberOf navigation property.|
|[Add memberOf](../api/group-post-memberof.md)|[directoryObject](../resources/directoryobject.md)|Add memberOf by posting to the memberOf collection.|
|[Remove memberOf](../api/group-delete-memberof.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List transitiveMembers](../api/group-list-transitivemembers.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the transitiveMembers navigation property.|
|[Add transitiveMembers](../api/group-post-transitivemembers.md)|[directoryObject](../resources/directoryobject.md)|Add transitiveMembers by posting to the transitiveMembers collection.|
|[Remove transitiveMembers](../api/group-delete-transitivemembers.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List transitiveMemberOf](../api/group-list-transitivememberof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the transitiveMemberOf navigation property.|
|[Add transitiveMemberOf](../api/group-post-transitivememberof.md)|[directoryObject](../resources/directoryobject.md)|Add transitiveMemberOf by posting to the transitiveMemberOf collection.|
|[Remove transitiveMemberOf](../api/group-delete-transitivememberof.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List createdOnBehalfOf](../api/group-list-createdonbehalfof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the createdOnBehalfOf navigation property.|
|[Add createdOnBehalfOf](../api/group-post-createdonbehalfof.md)|[directoryObject](../resources/directoryobject.md)|Add createdOnBehalfOf by posting to the createdOnBehalfOf collection.|
|[Remove createdOnBehalfOf](../api/group-delete-createdonbehalfof.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List owners](../api/group-list-owners.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the owners navigation property.|
|[Add owners](../api/group-post-owners.md)|[directoryObject](../resources/directoryobject.md)|Add owners by posting to the owners collection.|
|[Remove owners](../api/group-delete-owners.md)|None|Remove an [directoryObject](../resources/directoryobject.md) object.|
|[List settings](../api/group-list-settings.md)|[directorySetting](../resources/directorysetting.md) collection|Get the directorySettings from the settings navigation property.|
|[Create settings](../api/group-post-settings.md)|[directorySetting](../resources/directorysetting.md)|Create a new settings object.|
|[Delete settings](../api/group-delete-settings.md)|None|Delete a [directorySetting](../resources/directorysetting.md) object.|
|[Update settings](../api/group-update-settings.md)|[directorySetting](../resources/directorysetting.md)|Update the properties of a settings object.|
|[Get directorySetting](../api/directorysetting-get.md)|[directorySetting](../resources/directorysetting.md)|Read the properties and relationships of a [directorySetting](../resources/directorysetting.md) object.|
|[List endpoints](../api/group-list-endpoints.md)|[endpoint](../resources/endpoint.md) collection|Get the endpoints from the endpoints navigation property.|
|[Create endpoints](../api/group-post-endpoints.md)|[endpoint](../resources/endpoint.md)|Create a new endpoints object.|
|[Delete endpoints](../api/group-delete-endpoints.md)|None|Delete an [endpoint](../resources/endpoint.md) object.|
|[Update endpoints](../api/group-update-endpoints.md)|[endpoint](../resources/endpoint.md)|Update the properties of an endpoints object.|
|[Get endpoint](../api/endpoint-get.md)|[endpoint](../resources/endpoint.md)|Read the properties and relationships of an [endpoint](../resources/endpoint.md) object.|
|[List permissionGrants](../api/group-list-permissiongrants.md)|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) collection|Get the resourceSpecificPermissionGrants from the permissionGrants navigation property.|
|[Create permissionGrants](../api/group-post-permissiongrants.md)|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md)|Create a new permissionGrants object.|
|[Delete permissionGrants](../api/group-delete-permissiongrants.md)|None|Delete a [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object.|
|[Update permissionGrants](../api/group-update-permissiongrants.md)|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md)|Update the properties of a permissionGrants object.|
|[Get resourceSpecificPermissionGrant](../api/resourcespecificpermissiongrant-get.md)|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md)|Read the properties and relationships of a [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object.|
|[List conversations](../api/group-list-conversations.md)|[conversation](../resources/conversation.md) collection|Get the conversations from the conversations navigation property.|
|[Create conversations](../api/group-post-conversations.md)|[conversation](../resources/conversation.md)|Create a new conversations object.|
|[Delete conversations](../api/group-delete-conversations.md)|None|Delete a [conversation](../resources/conversation.md) object.|
|[Update conversations](../api/group-update-conversations.md)|[conversation](../resources/conversation.md)|Update the properties of a conversations object.|
|[Get conversation](../api/conversation-get.md)|[conversation](../resources/conversation.md)|Read the properties and relationships of a [conversation](../resources/conversation.md) object.|
|[List photos](../api/group-list-photos.md)|[profilePhoto](../resources/profilephoto.md) collection|Get the profilePhotoes from the photos navigation property.|
|[Create photos](../api/group-post-photos.md)|[profilePhoto](../resources/profilephoto.md)|Create a new photos object.|
|[Delete photos](../api/group-delete-photos.md)|None|Delete a [profilePhoto](../resources/profilephoto.md) object.|
|[Update photos](../api/group-update-photos.md)|[profilePhoto](../resources/profilephoto.md)|Update the properties of a photos object.|
|[Get profilePhoto](../api/profilephoto-get.md)|[profilePhoto](../resources/profilephoto.md)|Read the properties and relationships of a [profilePhoto](../resources/profilephoto.md) object.|
|[List acceptedSenders](../api/group-list-acceptedsenders.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the acceptedSenders navigation property.|
|[Create acceptedSenders](../api/group-post-acceptedsenders.md)|[directoryObject](../resources/directoryobject.md)|Create a new acceptedSenders object.|
|[Delete acceptedSenders](../api/group-delete-acceptedsenders.md)|None|Delete an [directoryObject](../resources/directoryobject.md) object.|
|[Update acceptedSenders](../api/group-update-acceptedsenders.md)|[directoryObject](../resources/directoryobject.md)|Update the properties of an acceptedSenders object.|
|[Get directoryObject](../api/directoryobject-get.md)|[directoryObject](../resources/directoryobject.md)|Read the properties and relationships of a [directoryObject](../resources/directoryobject.md) object.|
|[List rejectedSenders](../api/group-list-rejectedsenders.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the rejectedSenders navigation property.|
|[Create rejectedSenders](../api/group-post-rejectedsenders.md)|[directoryObject](../resources/directoryobject.md)|Create a new rejectedSenders object.|
|[Delete rejectedSenders](../api/group-delete-rejectedsenders.md)|None|Delete a [directoryObject](../resources/directoryobject.md) object.|
|[Update rejectedSenders](../api/group-update-rejectedsenders.md)|[directoryObject](../resources/directoryobject.md)|Update the properties of a rejectedSenders object.|
|[Get directoryObject](../api/directoryobject-get.md)|[directoryObject](../resources/directoryobject.md)|Read the properties and relationships of a [directoryObject](../resources/directoryobject.md) object.|
|[List threads](../api/group-list-threads.md)|[conversationThread](../resources/conversationthread.md) collection|Get the conversationThreads from the threads navigation property.|
|[Create threads](../api/group-post-threads.md)|[conversationThread](../resources/conversationthread.md)|Create a new threads object.|
|[Delete threads](../api/group-delete-threads.md)|None|Delete a [conversationThread](../resources/conversationthread.md) object.|
|[Update threads](../api/group-update-threads.md)|[conversationThread](../resources/conversationthread.md)|Update the properties of a threads object.|
|[Get conversationThread](../api/conversationthread-get.md)|[conversationThread](../resources/conversationthread.md)|Read the properties and relationships of a [conversationThread](../resources/conversationthread.md) object.|
|[List calendar](../api/group-list-calendar.md)|[calendar](../resources/calendar.md) collection|Get the calendars from the calendar navigation property.|
|[Create calendar](../api/group-post-calendar.md)|[calendar](../resources/calendar.md)|Create a new calendar object.|
|[Delete calendar](../api/group-delete-calendar.md)|None|Delete a [calendar](../resources/calendar.md) object.|
|[Update calendar](../api/group-update-calendar.md)|[calendar](../resources/calendar.md)|Update the properties of a calendar object.|
|[Get calendar](../api/calendar-get.md)|[calendar](../resources/calendar.md)|Read the properties and relationships of a [calendar](../resources/calendar.md) object.|
|[List calendarView](../api/group-list-calendarview.md)|[event](../resources/event.md) collection|Get the events from the calendarView navigation property.|
|[Create calendarView](../api/group-post-calendarview.md)|[event](../resources/event.md)|Create a new calendarView object.|
|[Delete calendarView](../api/group-delete-calendarview.md)|None|Delete a [event](../resources/event.md) object.|
|[Update calendarView](../api/group-update-calendarview.md)|[event](../resources/event.md)|Update the properties of a calendarView object.|
|[Get event](../api/event-get.md)|[event](../resources/event.md)|Read the properties and relationships of an [event](../resources/event.md) object.|
|[List events](../api/group-list-events.md)|[event](../resources/event.md) collection|Get the events from the events navigation property.|
|[Create events](../api/group-post-events.md)|[event](../resources/event.md)|Create a new events object.|
|[Delete events](../api/group-delete-events.md)|None|Delete an [event](../resources/event.md) object.|
|[Update events](../api/group-update-events.md)|[event](../resources/event.md)|Update the properties of an events object.|
|[Get event](../api/event-get.md)|[event](../resources/event.md)|Read the properties and relationships of an [event](../resources/event.md) object.|
|[List photo](../api/group-list-photo.md)|[profilePhoto](../resources/profilephoto.md) collection|Get the profilePhotoes from the photo navigation property.|
|[Create photo](../api/group-post-photo.md)|[profilePhoto](../resources/profilephoto.md)|Create a new photo object.|
|[Delete photo](../api/group-delete-photo.md)|None|Delete a [profilePhoto](../resources/profilephoto.md) object.|
|[Update photo](../api/group-update-photo.md)|[profilePhoto](../resources/profilephoto.md)|Update the properties of a photo object.|
|[Get profilePhoto](../api/profilephoto-get.md)|[profilePhoto](../resources/profilephoto.md)|Read the properties and relationships of a [profilePhoto](../resources/profilephoto.md) object.|
|[List drive](../api/group-list-drive.md)|[drive](../resources/drive.md) collection|Get the drives from the drive navigation property.|
|[Create drive](../api/group-post-drive.md)|[drive](../resources/drive.md)|Create a new drive object.|
|[Delete drive](../api/group-delete-drive.md)|None|Delete a [drive](../resources/drive.md) object.|
|[Update drive](../api/group-update-drive.md)|[drive](../resources/drive.md)|Update the properties of a drive object.|
|[Get drive](../api/drive-get.md)|[drive](../resources/drive.md)|Read the properties and relationships of a [drive](../resources/drive.md) object.|
|[List drives](../api/group-list-drives.md)|[drive](../resources/drive.md) collection|Get the drives from the drives navigation property.|
|[Create drives](../api/group-post-drives.md)|[drive](../resources/drive.md)|Create a new drives object.|
|[Delete drives](../api/group-delete-drives.md)|None|Delete a [drive](../resources/drive.md) object.|
|[Update drives](../api/group-update-drives.md)|[drive](../resources/drive.md)|Update the properties of a drives object.|
|[Get drive](../api/drive-get.md)|[drive](../resources/drive.md)|Read the properties and relationships of a [drive](../resources/drive.md) object.|
|[List sites](../api/group-list-sites.md)|[site](../resources/site.md) collection|Get the sites from the sites navigation property.|
|[Create sites](../api/group-post-sites.md)|[site](../resources/site.md)|Create a new sites object.|
|[Delete sites](../api/group-delete-sites.md)|None|Delete a [site](../resources/site.md) object.|
|[Update sites](../api/group-update-sites.md)|[site](../resources/site.md)|Update the properties of a sites object.|
|[Get site](../api/site-get.md)|[site](../resources/site.md)|Read the properties and relationships of a [site](../resources/site.md) object.|
|[List extensions](../api/group-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Create extensions](../api/group-post-extensions.md)|[extension](../resources/extension.md)|Create a new extensions object.|
|[Delete extensions](../api/group-delete-extensions.md)|None|Delete an [extension](../resources/extension.md) object.|
|[Update extensions](../api/group-update-extensions.md)|[extension](../resources/extension.md)|Update the properties of an extensions object.|
|[Get extension](../api/extension-get.md)|[extension](../resources/extension.md)|Read the properties and relationships of an [extension](../resources/extension.md) object.|
|[List groupLifecyclePolicies](../api/group-list-grouplifecyclepolicies.md)|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) collection|Get the groupLifecyclePolicies from the groupLifecyclePolicies navigation property.|
|[Create groupLifecyclePolicies](../api/group-post-grouplifecyclepolicies.md)|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)|Create a new groupLifecyclePolicies object.|
|[Delete groupLifecyclePolicies](../api/group-delete-grouplifecyclepolicies.md)|None|Delete a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.|
|[Update groupLifecyclePolicies](../api/group-update-grouplifecyclepolicies.md)|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)|Update the properties of a groupLifecyclePolicies object.|
|[Get groupLifecyclePolicy](../api/grouplifecyclepolicy-get.md)|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)|Read the properties and relationships of a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.|
|[List planner](../api/group-list-planner.md)|[plannerGroup](../resources/plannergroup.md) collection|Get the plannerGroups from the planner navigation property.|
|[Create planner](../api/group-post-planner.md)|[plannerGroup](../resources/plannergroup.md)|Create a new planner object.|
|[Delete planner](../api/group-delete-planner.md)|None|Delete a [plannerGroup](../resources/plannergroup.md) object.|
|[Update planner](../api/group-update-planner.md)|[plannerGroup](../resources/plannergroup.md)|Update the properties of a planner object.|
|[Get plannerGroup](../api/plannergroup-get.md)|[plannerGroup](../resources/plannergroup.md)|Read the properties and relationships of a [plannerGroup](../resources/plannergroup.md) object.|
|[List onenote](../api/group-list-onenote.md)|[onenote](../resources/onenote.md) collection|Get the onenotes from the onenote navigation property.|
|[Create onenote](../api/group-post-onenote.md)|[onenote](../resources/onenote.md)|Create a new onenote object.|
|[Delete onenote](../api/group-delete-onenote.md)|None|Delete an [onenote](../resources/onenote.md) object.|
|[Update onenote](../api/group-update-onenote.md)|[onenote](../resources/onenote.md)|Update the properties of an onenote object.|
|[Get onenote](../api/onenote-get.md)|[onenote](../resources/onenote.md)|Read the properties and relationships of an [onenote](../resources/onenote.md) object.|
|[List team](../api/group-list-team.md)|[team](../resources/team.md) collection|Get the teams from the team navigation property.|
|[Create team](../api/group-post-team.md)|[team](../resources/team.md)|Create a new team object.|
|[Delete team](../api/group-delete-team.md)|None|Delete a [team](../resources/team.md) object.|
|[Update team](../api/group-update-team.md)|[team](../resources/team.md)|Update the properties of a team object.|
|[Get team](../api/team-get.md)|[team](../resources/team.md)|Read the properties and relationships of a [team](../resources/team.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessType|groupAccessType|**TODO: Add Description**. Possible values are: `none`, `private`, `secret`, `public`.|
|allowExternalSenders|Boolean|**TODO: Add Description**|
|assignedLabels|[assignedLabel](../resources/assignedlabel.md) collection|**TODO: Add Description**|
|assignedLicenses|[assignedLicense](../resources/assignedlicense.md) collection|**TODO: Add Description**|
|autoSubscribeNewMembers|Boolean|**TODO: Add Description**|
|classification|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|groupTypes|String collection|**TODO: Add Description**|
|hasMembersWithLicenseErrors|Boolean|**TODO: Add Description**|
|hideFromAddressLists|Boolean|**TODO: Add Description**|
|hideFromOutlookClients|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isArchived|Boolean|**TODO: Add Description**|
|isAssignableToRole|Boolean|**TODO: Add Description**|
|isFavorite|Boolean|**TODO: Add Description**|
|isSubscribedByMail|Boolean|**TODO: Add Description**|
|licenseProcessingState|[licenseProcessingState](../resources/licenseprocessingstate.md)|**TODO: Add Description**|
|mail|String|**TODO: Add Description**|
|mailEnabled|Boolean|**TODO: Add Description**|
|mailNickname|String|**TODO: Add Description**|
|mdmAppId|String|**TODO: Add Description**|
|membershipRule|String|**TODO: Add Description**|
|membershipRuleProcessingState|String|**TODO: Add Description**|
|onPremisesDomainName|String|**TODO: Add Description**|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|onPremisesNetBiosName|String|**TODO: Add Description**|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](../resources/onpremisesprovisioningerror.md) collection|**TODO: Add Description**|
|onPremisesSamAccountName|String|**TODO: Add Description**|
|onPremisesSecurityIdentifier|String|**TODO: Add Description**|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description**|
|preferredDataLocation|String|**TODO: Add Description**|
|preferredLanguage|String|**TODO: Add Description**|
|proxyAddresses|String collection|**TODO: Add Description**|
|renewedDateTime|DateTimeOffset|**TODO: Add Description**|
|resourceBehaviorOptions|String collection|**TODO: Add Description**|
|resourceProvisioningOptions|String collection|**TODO: Add Description**|
|securityEnabled|Boolean|**TODO: Add Description**|
|securityIdentifier|String|**TODO: Add Description**|
|theme|String|**TODO: Add Description**|
|unseenConversationsCount|Int32|**TODO: Add Description**|
|unseenCount|Int32|**TODO: Add Description**|
|unseenMessagesCount|Int32|**TODO: Add Description**|
|visibility|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|acceptedSenders|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|appRoleAssignments|[appRoleAssignment](../resources/approleassignment.md) collection|**TODO: Add Description**|
|calendar|[calendar](../resources/calendar.md)|**TODO: Add Description**|
|calendarView|[event](../resources/event.md) collection|**TODO: Add Description**|
|conversations|[conversation](../resources/conversation.md) collection|**TODO: Add Description**|
|createdOnBehalfOf|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|drive|[drive](../resources/drive.md)|**TODO: Add Description**|
|drives|[drive](../resources/drive.md) collection|**TODO: Add Description**|
|endpoints|[endpoint](../resources/endpoint.md) collection|**TODO: Add Description**|
|events|[event](../resources/event.md) collection|**TODO: Add Description**|
|extensions|[extension](../resources/extension.md) collection|**TODO: Add Description**|
|groupLifecyclePolicies|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) collection|**TODO: Add Description**|
|memberOf|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|members|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|membersWithLicenseErrors|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|onenote|[onenote](../resources/onenote.md)|**TODO: Add Description**|
|owners|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|permissionGrants|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) collection|**TODO: Add Description**|
|photo|[profilePhoto](../resources/profilephoto.md)|**TODO: Add Description**|
|photos|[profilePhoto](../resources/profilephoto.md) collection|**TODO: Add Description**|
|planner|[plannerGroup](../resources/plannergroup.md)|**TODO: Add Description**|
|rejectedSenders|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|settings|[directorySetting](../resources/directorysetting.md) collection|**TODO: Add Description**|
|sites|[site](../resources/site.md) collection|**TODO: Add Description**|
|team|[team](../resources/team.md)|**TODO: Add Description**|
|threads|[conversationThread](../resources/conversationthread.md) collection|**TODO: Add Description**|
|transitiveMemberOf|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|transitiveMembers|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.group",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "assignedLabels": [
    {
      "@odata.type": "microsoft.graph.assignedLabel"
    }
  ],
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "classification": "String",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "groupTypes": [
    "String"
  ],
  "hasMembersWithLicenseErrors": "Boolean",
  "isAssignableToRole": "Boolean",
  "licenseProcessingState": {
    "@odata.type": "microsoft.graph.licenseProcessingState"
  },
  "mail": "String",
  "mailEnabled": "Boolean",
  "mailNickname": "String",
  "mdmAppId": "String",
  "membershipRule": "String",
  "membershipRuleProcessingState": "String",
  "onPremisesDomainName": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesNetBiosName": "String",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError"
    }
  ],
  "onPremisesSamAccountName": "String",
  "onPremisesSecurityIdentifier": "String",
  "onPremisesSyncEnabled": "Boolean",
  "preferredDataLocation": "String",
  "preferredLanguage": "String",
  "proxyAddresses": [
    "String"
  ],
  "renewedDateTime": "String (timestamp)",
  "resourceBehaviorOptions": [
    "String"
  ],
  "resourceProvisioningOptions": [
    "String"
  ],
  "securityEnabled": "Boolean",
  "securityIdentifier": "String",
  "theme": "String",
  "visibility": "String",
  "accessType": "String",
  "allowExternalSenders": "Boolean",
  "autoSubscribeNewMembers": "Boolean",
  "isFavorite": "Boolean",
  "isSubscribedByMail": "Boolean",
  "unseenCount": "Integer",
  "unseenConversationsCount": "Integer",
  "unseenMessagesCount": "Integer",
  "hideFromOutlookClients": "Boolean",
  "hideFromAddressLists": "Boolean",
  "isArchived": "Boolean"
}
```

