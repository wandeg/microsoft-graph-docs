---
title: "organization resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# organization resource type


Namespace: microsoft.graph




Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List organizations](../api/organization-list.md)|[organization](../resources/organization.md) collection|List properties and relationships of the [organization](../resources/organization.md) objects.|
|[Get organization](../api/organization-get.md)|[organization](../resources/organization.md)|Read properties and relationships of the [organization](../resources/organization.md) object.|
|[Create organization](../api/organization-post-organization.md)|[organization](../resources/organization.md)|Create a new [organization](../resources/organization.md) object.|
|[Delete organization](../api/organization-delete.md)|None|Deletes a [organization](../resources/organization.md).|
|[Update organization](../api/organization-update.md)|[organization](../resources/organization.md)|Update the properties of a [organization](../resources/organization.md) object.|
|[checkMemberGroups](../api/organization-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/organization-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/organization-getmembergroups.md)|String collection||
|[getMemberObjects](../api/organization-getmemberobjects.md)|String collection||
|[restore](../api/organization-restore.md)|[directoryObject](../resources/directoryobject.md)||
|[setMobileDeviceManagementAuthority](../api/organization-setmobiledevicemanagementauthority.md)|Int32||
|[getAppFamilyStatus](../api/organization-getappfamilystatus.md)|Enumeration||
|[getGroupSupportedAppFamilyStatus](../api/organization-getgroupsupportedappfamilystatus.md)|String||
|[getAppFamilyDetails](../api/organization-getappfamilydetails.md)|[appFamilyDetails](../resources/appfamilydetails.md)||
|[setAppFamilyStatus](../api/organization-setappfamilystatus.md)|None||
|[provisionAppFamily](../api/organization-provisionappfamily.md)|None||
|[List brandings](../api/organization-list-brandings.md)|[organizationalBranding](../resources/organizationalbranding.md) collection|Get the organizationalBrandings from the brandings navigation property.|
|[Add brandings](../api/organization-post-brandings.md)|[organizationalBranding](../resources/organizationalbranding.md)|Add brandings by posting to the brandings collection.|
|[List certificateBasedAuthConfiguration](../api/organization-list-certificatebasedauthconfiguration.md)|[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) collection|Get the certificateBasedAuthConfigurations from the certificateBasedAuthConfiguration navigation property.|
|[Create certificateBasedAuthConfiguration](../api/organization-post-certificatebasedauthconfiguration.md)|[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md)|Create certificateBasedAuthConfiguration by posting to the certificateBasedAuthConfiguration collection.|
|[List extensions](../api/organization-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Add extensions](../api/organization-post-extensions.md)|[extension](../resources/extension.md)|Add extensions by posting to the extensions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedPlans|[assignedPlan](../resources/assignedplan.md) collection||
|businessPhones|String collection||
|certificateConnectorSetting|[certificateConnectorSetting](../resources/certificateconnectorsetting.md)||
|city|String||
|country|String||
|countryLetterCode|String||
|createdDateTime|DateTimeOffset||
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|directorySizeQuota|[directorySizeQuota](../resources/directorysizequota.md)||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isMultipleDataLocationsForServicesEnabled|Boolean||
|marketingNotificationEmails|String collection||
|mobileDeviceManagementAuthority|Enumeration| Possible values are: `unknown`, `intune`, `sccm`, `office365`.|
|onPremisesLastSyncDateTime|DateTimeOffset||
|onPremisesSyncEnabled|Boolean||
|postalCode|String||
|preferredLanguage|String||
|privacyProfile|[privacyProfile](../resources/privacyprofile.md)||
|provisionedPlans|[provisionedPlan](../resources/provisionedplan.md) collection||
|securityComplianceNotificationMails|String collection||
|securityComplianceNotificationPhones|String collection||
|state|String||
|street|String||
|technicalNotificationMails|String collection||
|verifiedDomains|[verifiedDomain](../resources/verifieddomain.md) collection||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|brandings|[organizationalBranding](../resources/organizationalbranding.md) collection||
|certificateBasedAuthConfiguration|[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) collection||
|extensions|[extension](../resources/extension.md) collection||

## JSON representation
Here is a JSON representation of the resource.
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
      "@odata.type": "microsoft.graph.assignedPlan",
      "assignedDateTime": "String (timestamp)",
      "capabilityStatus": "String",
      "service": "String",
      "servicePlanId": "Guid"
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
    "@odata.type": "microsoft.graph.directorySizeQuota",
    "used": 1024,
    "total": 1024
  },
  "displayName": "String",
  "isMultipleDataLocationsForServicesEnabled": true,
  "marketingNotificationEmails": [
    "String"
  ],
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "postalCode": "String",
  "preferredLanguage": "String",
  "privacyProfile": {
    "@odata.type": "microsoft.graph.privacyProfile",
    "contactEmail": "String",
    "statementUrl": "String"
  },
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan",
      "provisioningStatus": "String"
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
      "@odata.type": "microsoft.graph.verifiedDomain",
      "capabilities": "String",
      "isDefault": true,
      "isInitial": true,
      "name": "String",
      "type": "String"
    }
  ],
  "mobileDeviceManagementAuthority": "String",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 1024,
    "certExpiryTime": "String (timestamp)",
    "enrollmentError": "String",
    "lastConnectorConnectionTime": "String (timestamp)",
    "connectorVersion": "String",
    "lastUploadVersion": 1024
  }
}
```

