---
title: "group resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# group resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List groups](../api/group-list.md)|[group](../resources/group.md) collection|Get a list of the [group](../resources/group.md) objects and their properties.|
|[Create group](../api/group-post-groups.md)|[group](../resources/group.md)|Create a new [group](../resources/group.md) object.|
|[Get group](../api/group-get.md)|[group](../resources/group.md)|Read the properties and relationships of a [group](../resources/group.md) object.|
|[Update group](../api/group-update.md)|[group](../resources/group.md)|Update the properties of a [group](../resources/group.md) object.|
|[Delete group](../api/group-delete.md)|None|Deletes a [group](../resources/group.md) object.|
|[delta](../api/group-delta.md)|[group](../resources/group.md) collection|**TODO: Add Description**|
|[checkMemberGroups](../api/group-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/group-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/group-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/group-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/group-restore.md)|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|[validateProperties](../api/group-validateproperties.md)|None|**TODO: Add Description**|
|[checkGrantedPermissionsForApp](../api/group-checkgrantedpermissionsforapp.md)|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) collection|**TODO: Add Description**|
|[assignLicense](../api/group-assignlicense.md)|[group](../resources/group.md)|**TODO: Add Description**|
|[List appRoleAssignments](../api/group-list-approleassignments.md)|[appRoleAssignment](../resources/approleassignment.md) collection|Get the appRoleAssignments from the appRoleAssignments navigation property.|
|[Create appRoleAssignments](../api/group-post-approleassignments.md)|[appRoleAssignment](../resources/approleassignment.md)|Create a new appRoleAssignments object.|
|[Get appRoleAssignments](../api/group-get-approleassignment.md)|[appRoleAssignment](../resources/approleassignment.md)|Read the properties and relationships of an [appRoleAssignment](../resources/approleassignment.md) object.|
|[Update appRoleAssignments](../api/group-update-approleassignments.md)|[appRoleAssignment](../resources/approleassignment.md)|Update the properties of an appRoleAssignments object.|
|[Delete appRoleAssignments](../api/group-delete-approleassignments.md)|None|Delete an [appRoleAssignment](../resources/approleassignment.md) object.|
|[List createdOnBehalfOf](../api/group-list-createdonbehalfof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the createdOnBehalfOf navigation property.|
|[Add createdOnBehalfOf](../api/group-post-createdonbehalfof.md)|[directoryObject](../resources/directoryobject.md)|Add createdOnBehalfOf by posting to the createdOnBehalfOf collection.|
|[Remove createdOnBehalfOf](../api/group-delete-createdonbehalfof.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List endpoints](../api/group-list-endpoints.md)|[endpoint](../resources/endpoint.md) collection|Get the endpoints from the endpoints navigation property.|
|[Create endpoints](../api/group-post-endpoints.md)|[endpoint](../resources/endpoint.md)|Create a new endpoints object.|
|[Get endpoints](../api/group-get-endpoint.md)|[endpoint](../resources/endpoint.md)|Read the properties and relationships of an [endpoint](../resources/endpoint.md) object.|
|[Update endpoints](../api/group-update-endpoints.md)|[endpoint](../resources/endpoint.md)|Update the properties of an endpoints object.|
|[Delete endpoints](../api/group-delete-endpoints.md)|None|Delete an [endpoint](../resources/endpoint.md) object.|
|[List memberOf](../api/group-list-memberof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the memberOf navigation property.|
|[Add memberOf](../api/group-post-memberof.md)|[directoryObject](../resources/directoryobject.md)|Add memberOf by posting to the memberOf collection.|
|[Remove memberOf](../api/group-delete-memberof.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List members](../api/group-list-members.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the members navigation property.|
|[Add members](../api/group-post-members.md)|[directoryObject](../resources/directoryobject.md)|Add members by posting to the members collection.|
|[Remove members](../api/group-delete-members.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List membersWithLicenseErrors](../api/group-list-memberswithlicenseerrors.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the membersWithLicenseErrors navigation property.|
|[Add membersWithLicenseErrors](../api/group-post-memberswithlicenseerrors.md)|[directoryObject](../resources/directoryobject.md)|Add membersWithLicenseErrors by posting to the membersWithLicenseErrors collection.|
|[Remove membersWithLicenseErrors](../api/group-delete-memberswithlicenseerrors.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List owners](../api/group-list-owners.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the owners navigation property.|
|[Add owners](../api/group-post-owners.md)|[directoryObject](../resources/directoryobject.md)|Add owners by posting to the owners collection.|
|[Remove owners](../api/group-delete-owners.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List permissionGrants](../api/group-list-permissiongrants.md)|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) collection|Get the resourceSpecificPermissionGrants from the permissionGrants navigation property.|
|[Create permissionGrants](../api/group-post-permissiongrants.md)|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md)|Create a new permissionGrants object.|
|[Get permissionGrants](../api/group-get-resourcespecificpermissiongrant.md)|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md)|Read the properties and relationships of a [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object.|
|[Update permissionGrants](../api/group-update-permissiongrants.md)|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md)|Update the properties of a permissionGrants object.|
|[Delete permissionGrants](../api/group-delete-permissiongrants.md)|None|Delete a [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object.|
|[List settings](../api/group-list-settings.md)|[directorySetting](../resources/directorysetting.md) collection|Get the directorySettings from the settings navigation property.|
|[Create settings](../api/group-post-settings.md)|[directorySetting](../resources/directorysetting.md)|Create a new settings object.|
|[Get settings](../api/group-get-directorysetting.md)|[directorySetting](../resources/directorysetting.md)|Read the properties and relationships of a [directorySetting](../resources/directorysetting.md) object.|
|[Update settings](../api/group-update-settings.md)|[directorySetting](../resources/directorysetting.md)|Update the properties of a settings object.|
|[Delete settings](../api/group-delete-settings.md)|None|Delete a [directorySetting](../resources/directorysetting.md) object.|
|[List transitiveMemberOf](../api/group-list-transitivememberof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the transitiveMemberOf navigation property.|
|[Add transitiveMemberOf](../api/group-post-transitivememberof.md)|[directoryObject](../resources/directoryobject.md)|Add transitiveMemberOf by posting to the transitiveMemberOf collection.|
|[Remove transitiveMemberOf](../api/group-delete-transitivememberof.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List transitiveMembers](../api/group-list-transitivemembers.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the transitiveMembers navigation property.|
|[Add transitiveMembers](../api/group-post-transitivemembers.md)|[directoryObject](../resources/directoryobject.md)|Add transitiveMembers by posting to the transitiveMembers collection.|
|[Remove transitiveMembers](../api/group-delete-transitivemembers.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedLabels|[assignedLabel](../resources/assignedlabel.md) collection|**TODO: Add Description**|
|assignedLicenses|[assignedLicense](../resources/assignedlicense.md) collection|**TODO: Add Description**|
|classification|String|**TODO: Add Description**|
|createdByAppId|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|groupTypes|String collection|**TODO: Add Description**|
|hasMembersWithLicenseErrors|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isAssignableToRole|Boolean|**TODO: Add Description**|
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
|visibility|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appRoleAssignments|[appRoleAssignment](../resources/approleassignment.md) collection|**TODO: Add Description**|
|createdOnBehalfOf|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|endpoints|[endpoint](../resources/endpoint.md) collection|**TODO: Add Description**|
|memberOf|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|members|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|membersWithLicenseErrors|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|owners|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|permissionGrants|[resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) collection|**TODO: Add Description**|
|settings|[directorySetting](../resources/directorysetting.md) collection|**TODO: Add Description**|
|transitiveMemberOf|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|transitiveMembers|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "createdByAppId": "String",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "expirationDateTime": "String (timestamp)",
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
  "visibility": "String"
}
```

