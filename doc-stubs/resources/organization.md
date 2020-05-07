---
title: "organization resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# organization resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List organizations](../api/organization-list.md)|[organization](../resources/organization.md) collection|Get a list of the [organization](../resources/organization.md) objects and their properties.|
|[Get organization](../api/organization-get.md)|[organization](../resources/organization.md)|Read the properties and relationships of an [organization](../resources/organization.md) object.|
|[Create organization](../api/organization-post-organization.md)|[organization](../resources/organization.md)|Create a new [organization](../resources/organization.md) object.|
|[Delete organization](../api/organization-delete.md)|None|Deletes an [organization](../resources/organization.md) object.|
|[Update organization](../api/organization-update.md)|[organization](../resources/organization.md)|Update the properties of an [organization](../resources/organization.md) object.|
|[checkMemberGroups](../api/organization-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/organization-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/organization-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/organization-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/organization-restore.md)|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|[setMobileDeviceManagementAuthority](../api/organization-setmobiledevicemanagementauthority.md)|Int32|**TODO: Add Description**|
|[getAppFamilyStatus](../api/organization-getappfamilystatus.md)|appFamilyLinkedInStatus|**TODO: Add Description**|
|[getGroupSupportedAppFamilyStatus](../api/organization-getgroupsupportedappfamilystatus.md)|String|**TODO: Add Description**|
|[getAppFamilyDetails](../api/organization-getappfamilydetails.md)|[appFamilyDetails](../resources/appfamilydetails.md)|**TODO: Add Description**|
|[setAppFamilyStatus](../api/organization-setappfamilystatus.md)|None|**TODO: Add Description**|
|[provisionAppFamily](../api/organization-provisionappfamily.md)|None|**TODO: Add Description**|
|[List brandings](../api/organization-list-brandings.md)|[organizationalBranding](../resources/organizationalbranding.md) collection|Get the organizationalBrandings from the brandings navigation property.|
|[Create brandings](../api/organization-post-brandings.md)|[organizationalBranding](../resources/organizationalbranding.md)|Create a new brandings object.|
|[Delete brandings](../api/organization-delete-brandings.md)|None|Delete a [organizationalBranding](../resources/organizationalbranding.md) object.|
|[Update brandings](../api/organization-update-brandings.md)|[organizationalBranding](../resources/organizationalbranding.md)|Update the properties of a brandings object.|
|[Get organizationalBranding](../api/organizationalbranding-get.md)|[organizationalBranding](../resources/organizationalbranding.md)|Read the properties and relationships of an [organizationalBranding](../resources/organizationalbranding.md) object.|
|[List certificateBasedAuthConfiguration](../api/organization-list-certificatebasedauthconfiguration.md)|[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) collection|Get the certificateBasedAuthConfigurations from the certificateBasedAuthConfiguration navigation property.|
|[Add certificateBasedAuthConfiguration](../api/organization-post-certificatebasedauthconfiguration.md)|[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md)|Add certificateBasedAuthConfiguration by posting to the certificateBasedAuthConfiguration collection.|
|[Remove certificateBasedAuthConfiguration](../api/organization-delete-certificatebasedauthconfiguration.md)|None|Remove a [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.|
|[List extensions](../api/organization-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Create extensions](../api/organization-post-extensions.md)|[extension](../resources/extension.md)|Create a new extensions object.|
|[Delete extensions](../api/organization-delete-extensions.md)|None|Delete an [extension](../resources/extension.md) object.|
|[Update extensions](../api/organization-update-extensions.md)|[extension](../resources/extension.md)|Update the properties of an extensions object.|
|[Get extension](../api/extension-get.md)|[extension](../resources/extension.md)|Read the properties and relationships of an [extension](../resources/extension.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedPlans|[assignedPlan](../resources/assignedplan.md) collection|**TODO: Add Description**|
|businessPhones|String collection|**TODO: Add Description**|
|certificateConnectorSetting|[certificateConnectorSetting](../resources/certificateconnectorsetting.md)|**TODO: Add Description**|
|city|String|**TODO: Add Description**|
|country|String|**TODO: Add Description**|
|countryLetterCode|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|directorySizeQuota|[directorySizeQuota](../resources/directorysizequota.md)|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isMultipleDataLocationsForServicesEnabled|Boolean|**TODO: Add Description**|
|marketingNotificationEmails|String collection|**TODO: Add Description**|
|mobileDeviceManagementAuthority|mdmAuthority|**TODO: Add Description**. Possible values are: `unknown`, `intune`, `sccm`, `office365`.|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description**|
|postalCode|String|**TODO: Add Description**|
|preferredLanguage|String|**TODO: Add Description**|
|privacyProfile|[privacyProfile](../resources/privacyprofile.md)|**TODO: Add Description**|
|provisionedPlans|[provisionedPlan](../resources/provisionedplan.md) collection|**TODO: Add Description**|
|securityComplianceNotificationMails|String collection|**TODO: Add Description**|
|securityComplianceNotificationPhones|String collection|**TODO: Add Description**|
|state|String|**TODO: Add Description**|
|street|String|**TODO: Add Description**|
|technicalNotificationMails|String collection|**TODO: Add Description**|
|verifiedDomains|[verifiedDomain](../resources/verifieddomain.md) collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|brandings|[organizationalBranding](../resources/organizationalbranding.md) collection|**TODO: Add Description**|
|certificateBasedAuthConfiguration|[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) collection|**TODO: Add Description**|
|extensions|[extension](../resources/extension.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organization",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "businessPhones": [
    "String"
  ],
  "city": "String",
  "country": "String",
  "countryLetterCode": "String",
  "createdDateTime": "String (timestamp)",
  "directorySizeQuota": {
    "@odata.type": "microsoft.graph.directorySizeQuota"
  },
  "displayName": "String",
  "isMultipleDataLocationsForServicesEnabled": "Boolean",
  "marketingNotificationEmails": [
    "String"
  ],
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": "Boolean",
  "postalCode": "String",
  "preferredLanguage": "String",
  "privacyProfile": {
    "@odata.type": "microsoft.graph.privacyProfile"
  },
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "securityComplianceNotificationMails": [
    "String"
  ],
  "securityComplianceNotificationPhones": [
    "String"
  ],
  "state": "String",
  "street": "String",
  "technicalNotificationMails": [
    "String"
  ],
  "verifiedDomains": [
    {
      "@odata.type": "microsoft.graph.verifiedDomain"
    }
  ],
  "mobileDeviceManagementAuthority": "String",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting"
  }
}
```

