---
title: "group resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# group resource type


Namespace: microsoft.graph

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groups](../api/group-list.md)|[group](../resources/group.md) collection|Get a list of the [group](../resources/group.md) objects and their properties.|
|[Get group](../api/group-get.md)|[group](../resources/group.md)|Read properties and relationships of a [group](../resources/group.md) object.|
|[Create group](../api/group-post-groups.md)|[group](../resources/group.md)|Create a new [group](../resources/group.md) object.|
|[Delete group](../api/group-delete.md)|None|Deletes a [group](../resources/group.md).|
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
|[List members](../api/group-list-members.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the members navigation property.|
|[Add members](../api/group-post-members.md)|[directoryObject](../resources/directoryobject.md)|Add members by posting to the members collection.|
|[List membersWithLicenseErrors](../api/group-list-memberswithlicenseerrors.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the membersWithLicenseErrors navigation property.|
|[Add membersWithLicenseErrors](../api/group-post-memberswithlicenseerrors.md)|[directoryObject](../resources/directoryobject.md)|Add membersWithLicenseErrors by posting to the membersWithLicenseErrors collection.|
|[List memberOf](../api/group-list-memberof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the memberOf navigation property.|
|[Add memberOf](../api/group-post-memberof.md)|[directoryObject](../resources/directoryobject.md)|Add memberOf by posting to the memberOf collection.|
|[List transitiveMembers](../api/group-list-transitivemembers.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the transitiveMembers navigation property.|
|[Add transitiveMembers](../api/group-post-transitivemembers.md)|[directoryObject](../resources/directoryobject.md)|Add transitiveMembers by posting to the transitiveMembers collection.|
|[List transitiveMemberOf](../api/group-list-transitivememberof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the transitiveMemberOf navigation property.|
|[Add transitiveMemberOf](../api/group-post-transitivememberof.md)|[directoryObject](../resources/directoryobject.md)|Add transitiveMemberOf by posting to the transitiveMemberOf collection.|
|[Get directoryObject](../api/directoryobject-get.md)|[directoryObject](../resources/directoryobject.md)|Read properties and relationships of a [directoryObject](../resources/directoryobject.md) object.|
|[List owners](../api/group-list-owners.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the owners navigation property.|
|[Add owners](../api/group-post-owners.md)|[directoryObject](../resources/directoryobject.md)|Add owners by posting to the owners collection.|
|[List settings](../api/group-list-settings.md)|[directorySetting](../resources/directorysetting.md) collection|Get the directorySettings from the settings navigation property.|
|[Create settings](../api/group-post-settings.md)|[directorySetting](../resources/directorysetting.md)|Create a new settings object.|
|[List endpoints](../api/group-list-endpoints.md)|[endpoint](../resources/endpoint.md) collection|Get the endpoints from the endpoints navigation property.|
|[Create endpoints](../api/group-post-endpoints.md)|[endpoint](../resources/endpoint.md)|Create a new endpoints object.|
|[List permissionGrants](../api/group-list-permissiongrants.md)|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) collection|Get the resourceSpecificPermissionGrants from the permissionGrants navigation property.|
|[Create permissionGrants](../api/group-post-permissiongrants.md)|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md)|Create a new permissionGrants object.|
|[List conversations](../api/group-list-conversations.md)|[conversation](../resources/conversation.md) collection|Get the conversations from the conversations navigation property.|
|[Create conversations](../api/group-post-conversations.md)|[conversation](../resources/conversation.md)|Create a new conversations object.|
|[List photos](../api/group-list-photos.md)|[profilePhoto](../resources/profilephoto.md) collection|Get the profilePhotoes from the photos navigation property.|
|[Create photos](../api/group-post-photos.md)|[profilePhoto](../resources/profilephoto.md)|Create a new photos object.|
|[List acceptedSenders](../api/group-list-acceptedsenders.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the acceptedSenders navigation property.|
|[Create acceptedSenders](../api/group-post-acceptedsenders.md)|[directoryObject](../resources/directoryobject.md)|Create a new acceptedSenders object.|
|[List rejectedSenders](../api/group-list-rejectedsenders.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the rejectedSenders navigation property.|
|[Create rejectedSenders](../api/group-post-rejectedsenders.md)|[directoryObject](../resources/directoryobject.md)|Create a new rejectedSenders object.|
|[List threads](../api/group-list-threads.md)|[conversationThread](../resources/conversationthread.md) collection|Get the conversationThreads from the threads navigation property.|
|[Create threads](../api/group-post-threads.md)|[conversationThread](../resources/conversationthread.md)|Create a new threads object.|
|[Get calendar](../api/calendar-get.md)|[calendar](../resources/calendar.md)|Read properties and relationships of a [calendar](../resources/calendar.md) object.|
|[List calendarView](../api/group-list-calendarview.md)|[event](../resources/event.md) collection|Get the events from the calendarView navigation property.|
|[Create calendarView](../api/group-post-calendarview.md)|[event](../resources/event.md)|Create a new calendarView object.|
|[List events](../api/group-list-events.md)|[event](../resources/event.md) collection|Get the events from the events navigation property.|
|[Create events](../api/group-post-events.md)|[event](../resources/event.md)|Create a new events object.|
|[Get profilePhoto](../api/profilephoto-get.md)|[profilePhoto](../resources/profilephoto.md)|Read properties and relationships of a [profilePhoto](../resources/profilephoto.md) object.|
|[Get drive](../api/drive-get.md)|[drive](../resources/drive.md)|Read properties and relationships of a [drive](../resources/drive.md) object.|
|[List drives](../api/group-list-drives.md)|[drive](../resources/drive.md) collection|Get the drives from the drives navigation property.|
|[Create drives](../api/group-post-drives.md)|[drive](../resources/drive.md)|Create a new drives object.|
|[List sites](../api/group-list-sites.md)|[site](../resources/site.md) collection|Get the sites from the sites navigation property.|
|[Create sites](../api/group-post-sites.md)|[site](../resources/site.md)|Create a new sites object.|
|[List extensions](../api/group-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Create extensions](../api/group-post-extensions.md)|[extension](../resources/extension.md)|Create a new extensions object.|
|[List groupLifecyclePolicies](../api/group-list-grouplifecyclepolicies.md)|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) collection|Get the groupLifecyclePolicies from the groupLifecyclePolicies navigation property.|
|[Create groupLifecyclePolicies](../api/group-post-grouplifecyclepolicies.md)|[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)|Create a new groupLifecyclePolicies object.|
|[Get plannerGroup](../api/plannergroup-get.md)|[plannerGroup](../resources/plannergroup.md)|Read properties and relationships of a [plannerGroup](../resources/plannergroup.md) object.|
|[Get onenote](../api/onenote-get.md)|[onenote](../resources/onenote.md)|Read properties and relationships of an [onenote](../resources/onenote.md) object.|
|[Get team](../api/team-get.md)|[team](../resources/team.md)|Read properties and relationships of a [team](../resources/team.md) object.|
|[List joinedGroups](../api/user-list-joinedgroups.md)|[group](../resources/group.md) collection|Get the groups from the joinedGroups navigation property.|
|[Create joinedGroups](../api/user-post-joinedgroups.md)|[group](../resources/group.md)|Create a new joinedGroups object.|

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
      "@odata.type": "microsoft.graph.assignedLabel",
      "labelId": "String"
    }
  ],
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense",
      "disabledPlans": [
        "Guid"
      ],
      "skuId": "Guid"
    }
  ],
  "classification": "String",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "groupTypes": [
    "String"
  ],
  "hasMembersWithLicenseErrors": true,
  "isAssignableToRole": true,
  "licenseProcessingState": {
    "@odata.type": "microsoft.graph.licenseProcessingState",
    "state": "String"
  },
  "mail": "String",
  "mailEnabled": true,
  "mailNickname": "String",
  "mdmAppId": "String",
  "membershipRule": "String",
  "membershipRuleProcessingState": "String",
  "onPremisesDomainName": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesNetBiosName": "String",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "String",
      "category": "String",
      "propertyCausingError": "String",
      "occurredDateTime": "String (timestamp)"
    }
  ],
  "onPremisesSamAccountName": "String",
  "onPremisesSecurityIdentifier": "String",
  "onPremisesSyncEnabled": true,
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
  "securityEnabled": true,
  "securityIdentifier": "String",
  "theme": "String",
  "visibility": "String",
  "accessType": "String",
  "allowExternalSenders": true,
  "autoSubscribeNewMembers": true,
  "isFavorite": true,
  "isSubscribedByMail": true,
  "unseenCount": 1024,
  "unseenConversationsCount": 1024,
  "unseenMessagesCount": 1024,
  "hideFromOutlookClients": true,
  "hideFromAddressLists": true,
  "isArchived": true
}
```

