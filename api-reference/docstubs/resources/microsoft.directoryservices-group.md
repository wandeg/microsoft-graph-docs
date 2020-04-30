---
title: "group resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# group resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groups](../api/microsoft.directoryservices-group-list.md)|[group](../resources/microsoft.directoryservices-group.md) collection|Get a list of the [group](../resources/group.md) objects and their properties.|
|[Get group](../api/microsoft.directoryservices-group-get.md)|[group](../resources/microsoft.directoryservices-group.md)|Read properties and relationships of a [group](../resources/microsoft.directoryservices-group.md) object.|
|[Create group](../api/microsoft.directoryservices-group-post-groups.md)|[group](../resources/microsoft.directoryservices-group.md)|Create a new [group](../resources/microsoft.directoryservices-group.md) object.|
|[Delete group](../api/microsoft.directoryservices-group-delete.md)|None|Deletes a [group](../resources/microsoft.directoryservices-group.md).|
|[Update group](../api/microsoft.directoryservices-group-update.md)|[group](../resources/microsoft.directoryservices-group.md)|Update the properties of a [group](../resources/microsoft.directoryservices-group.md) object.|
|[delta](../api/microsoft.directoryservices-group-delta.md)|[group](../resources/microsoft.directoryservices-group.md) collection|**TODO: Add Description**|
|[checkMemberGroups](../api/microsoft.directoryservices-group-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/microsoft.directoryservices-group-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/microsoft.directoryservices-group-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/microsoft.directoryservices-group-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[validateProperties](../api/microsoft.directoryservices-group-validateproperties.md)|None|**TODO: Add Description**|
|[restore](../api/microsoft.directoryservices-group-restore.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|**TODO: Add Description**|
|[grantResourceSpecificConsent](../api/microsoft.directoryservices-group-grantresourcespecificconsent.md)|None|**TODO: Add Description**|
|[revokeResourceSpecificConsent](../api/microsoft.directoryservices-group-revokeresourcespecificconsent.md)|None|**TODO: Add Description**|
|[checkGrantedPermissionsForApp](../api/microsoft.directoryservices-group-checkgrantedpermissionsforapp.md)|[resourceSpecificPermissionGrant](../resources/microsoft.directoryservices-resourcespecificpermissiongrant.md) collection|**TODO: Add Description**|
|[assignLicense](../api/microsoft.directoryservices-group-assignlicense.md)|[group](../resources/microsoft.directoryservices-group.md)|**TODO: Add Description**|
|[List appRoleAssignments](../api/microsoft.directoryservices-group-list-approleassignments.md)|[appRoleAssignment](../resources/microsoft.directoryservices-approleassignment.md) collection|Get the appRoleAssignments from the appRoleAssignments navigation property.|
|[Create appRoleAssignments](../api/microsoft.directoryservices-group-post-approleassignments.md)|[appRoleAssignment](../resources/microsoft.directoryservices-approleassignment.md)|Create a new appRoleAssignments object.|
|[Delete appRoleAssignments](../api/microsoft.directoryservices-group-delete-approleassignments.md)|None|Delete an appRoleAssignments object.|
|[Update appRoleAssignments](../api/microsoft.directoryservices-group-update-approleassignments.md)|[appRoleAssignment](../resources/microsoft.directoryservices-approleassignment.md)|Update the properties of an appRoleAssignments object.|
|[Get appRoleAssignment](../api/microsoft.directoryservices-approleassignment-get.md)|[appRoleAssignment](../resources/microsoft.directoryservices-approleassignment.md)|Read properties and relationships of an [appRoleAssignment](../resources/microsoft.directoryservices-approleassignment.md) object.|
|[List members](../api/microsoft.directoryservices-group-list-members.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the members navigation property.|
|[Add members](../api/microsoft.directoryservices-group-post-members.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add members by posting to the members collection.|
|[Remove members](../api/microsoft.directoryservices-group-delete-members.md)|None|Remove a members object.|
|[List membersWithLicenseErrors](../api/microsoft.directoryservices-group-list-memberswithlicenseerrors.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the membersWithLicenseErrors navigation property.|
|[Add membersWithLicenseErrors](../api/microsoft.directoryservices-group-post-memberswithlicenseerrors.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add membersWithLicenseErrors by posting to the membersWithLicenseErrors collection.|
|[Remove membersWithLicenseErrors](../api/microsoft.directoryservices-group-delete-memberswithlicenseerrors.md)|None|Remove a membersWithLicenseErrors object.|
|[List memberOf](../api/microsoft.directoryservices-group-list-memberof.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the memberOf navigation property.|
|[Add memberOf](../api/microsoft.directoryservices-group-post-memberof.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add memberOf by posting to the memberOf collection.|
|[Remove memberOf](../api/microsoft.directoryservices-group-delete-memberof.md)|None|Remove a memberOf object.|
|[List transitiveMembers](../api/microsoft.directoryservices-group-list-transitivemembers.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the transitiveMembers navigation property.|
|[Add transitiveMembers](../api/microsoft.directoryservices-group-post-transitivemembers.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add transitiveMembers by posting to the transitiveMembers collection.|
|[Remove transitiveMembers](../api/microsoft.directoryservices-group-delete-transitivemembers.md)|None|Remove a transitiveMembers object.|
|[List transitiveMemberOf](../api/microsoft.directoryservices-group-list-transitivememberof.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the transitiveMemberOf navigation property.|
|[Add transitiveMemberOf](../api/microsoft.directoryservices-group-post-transitivememberof.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add transitiveMemberOf by posting to the transitiveMemberOf collection.|
|[Remove transitiveMemberOf](../api/microsoft.directoryservices-group-delete-transitivememberof.md)|None|Remove a transitiveMemberOf object.|
|[List createdOnBehalfOf](../api/microsoft.directoryservices-group-list-createdonbehalfof.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the createdOnBehalfOf navigation property.|
|[Add createdOnBehalfOf](../api/microsoft.directoryservices-group-post-createdonbehalfof.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add createdOnBehalfOf by posting to the createdOnBehalfOf collection.|
|[Remove createdOnBehalfOf](../api/microsoft.directoryservices-group-delete-createdonbehalfof.md)|None|Remove a createdOnBehalfOf object.|
|[List owners](../api/microsoft.directoryservices-group-list-owners.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the owners navigation property.|
|[Add owners](../api/microsoft.directoryservices-group-post-owners.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add owners by posting to the owners collection.|
|[Remove owners](../api/microsoft.directoryservices-group-delete-owners.md)|None|Remove an owners object.|
|[List settings](../api/microsoft.directoryservices-group-list-settings.md)|[directorySetting](../resources/microsoft.directoryservices-directorysetting.md) collection|Get the directorySettings from the settings navigation property.|
|[Create settings](../api/microsoft.directoryservices-group-post-settings.md)|[directorySetting](../resources/microsoft.directoryservices-directorysetting.md)|Create a new settings object.|
|[Delete settings](../api/microsoft.directoryservices-group-delete-settings.md)|None|Delete a settings object.|
|[Update settings](../api/microsoft.directoryservices-group-update-settings.md)|[directorySetting](../resources/microsoft.directoryservices-directorysetting.md)|Update the properties of a settings object.|
|[Get directorySetting](../api/microsoft.directoryservices-directorysetting-get.md)|[directorySetting](../resources/microsoft.directoryservices-directorysetting.md)|Read properties and relationships of a [directorySetting](../resources/microsoft.directoryservices-directorysetting.md) object.|
|[List endpoints](../api/microsoft.directoryservices-group-list-endpoints.md)|[endpoint](../resources/microsoft.directoryservices-endpoint.md) collection|Get the endpoints from the endpoints navigation property.|
|[Create endpoints](../api/microsoft.directoryservices-group-post-endpoints.md)|[endpoint](../resources/microsoft.directoryservices-endpoint.md)|Create a new endpoints object.|
|[Delete endpoints](../api/microsoft.directoryservices-group-delete-endpoints.md)|None|Delete an endpoints object.|
|[Update endpoints](../api/microsoft.directoryservices-group-update-endpoints.md)|[endpoint](../resources/microsoft.directoryservices-endpoint.md)|Update the properties of an endpoints object.|
|[Get endpoint](../api/microsoft.directoryservices-endpoint-get.md)|[endpoint](../resources/microsoft.directoryservices-endpoint.md)|Read properties and relationships of an [endpoint](../resources/microsoft.directoryservices-endpoint.md) object.|
|[List permissionGrants](../api/microsoft.directoryservices-group-list-permissiongrants.md)|[resourceSpecificPermissionGrant](../resources/microsoft.directoryservices-resourcespecificpermissiongrant.md) collection|Get the resourceSpecificPermissionGrants from the permissionGrants navigation property.|
|[Create permissionGrants](../api/microsoft.directoryservices-group-post-permissiongrants.md)|[resourceSpecificPermissionGrant](../resources/microsoft.directoryservices-resourcespecificpermissiongrant.md)|Create a new permissionGrants object.|
|[Delete permissionGrants](../api/microsoft.directoryservices-group-delete-permissiongrants.md)|None|Delete a permissionGrants object.|
|[Update permissionGrants](../api/microsoft.directoryservices-group-update-permissiongrants.md)|[resourceSpecificPermissionGrant](../resources/microsoft.directoryservices-resourcespecificpermissiongrant.md)|Update the properties of a permissionGrants object.|
|[Get resourceSpecificPermissionGrant](../api/microsoft.directoryservices-resourcespecificpermissiongrant-get.md)|[resourceSpecificPermissionGrant](../resources/microsoft.directoryservices-resourcespecificpermissiongrant.md)|Read properties and relationships of a [resourceSpecificPermissionGrant](../resources/microsoft.directoryservices-resourcespecificpermissiongrant.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedLabels|[assignedLabel](../resources/microsoft.directoryservices-assignedlabel.md) collection|**TODO: Add Description**|
|assignedLicenses|[assignedLicense](../resources/microsoft.directoryservices-assignedlicense.md) collection|**TODO: Add Description**|
|classification|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|groupTypes|String collection|**TODO: Add Description**|
|hasMembersWithLicenseErrors|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|isAssignableToRole|Boolean|**TODO: Add Description**|
|licenseProcessingState|[licenseProcessingState](../resources/microsoft.directoryservices-licenseprocessingstate.md)|**TODO: Add Description**|
|mail|String|**TODO: Add Description**|
|mailEnabled|Boolean|**TODO: Add Description**|
|mailNickname|String|**TODO: Add Description**|
|mdmAppId|String|**TODO: Add Description**|
|membershipRule|String|**TODO: Add Description**|
|membershipRuleProcessingState|String|**TODO: Add Description**|
|onPremisesDomainName|String|**TODO: Add Description**|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|onPremisesNetBiosName|String|**TODO: Add Description**|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](../resources/microsoft.directoryservices-onpremisesprovisioningerror.md) collection|**TODO: Add Description**|
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
|appRoleAssignments|[appRoleAssignment](../resources/microsoft.directoryservices-approleassignment.md) collection|**TODO: Add Description**|
|createdOnBehalfOf|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|**TODO: Add Description**|
|endpoints|[endpoint](../resources/microsoft.directoryservices-endpoint.md) collection|**TODO: Add Description**|
|memberOf|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|
|members|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|
|membersWithLicenseErrors|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|
|owners|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|
|permissionGrants|[resourceSpecificPermissionGrant](../resources/microsoft.directoryservices-resourcespecificpermissiongrant.md) collection|**TODO: Add Description**|
|settings|[directorySetting](../resources/microsoft.directoryservices-directorysetting.md) collection|**TODO: Add Description**|
|transitiveMemberOf|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|
|transitiveMembers|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.group",
  "baseType": "Microsoft.DirectoryServices.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.group",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "assignedLabels": [
    {
      "@odata.type": "Microsoft.DirectoryServices.assignedLabel",
      "labelId": "String"
    }
  ],
  "assignedLicenses": [
    {
      "@odata.type": "Microsoft.DirectoryServices.assignedLicense",
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
    "@odata.type": "Microsoft.DirectoryServices.licenseProcessingState",
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
      "@odata.type": "Microsoft.DirectoryServices.onPremisesProvisioningError",
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
  "visibility": "String"
}
```

