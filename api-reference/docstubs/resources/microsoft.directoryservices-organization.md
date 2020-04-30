---
title: "organization resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# organization resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List organizations](../api/microsoft.directoryservices-organization-list.md)|[organization](../resources/microsoft.directoryservices-organization.md) collection|Get a list of the [organization](../resources/organization.md) objects and their properties.|
|[Get organization](../api/microsoft.directoryservices-organization-get.md)|[organization](../resources/microsoft.directoryservices-organization.md)|Read properties and relationships of an [organization](../resources/microsoft.directoryservices-organization.md) object.|
|[Create organization](../api/microsoft.directoryservices-organization-post-organization.md)|[organization](../resources/microsoft.directoryservices-organization.md)|Create a new [organization](../resources/microsoft.directoryservices-organization.md) object.|
|[Delete organization](../api/microsoft.directoryservices-organization-delete.md)|None|Deletes an [organization](../resources/microsoft.directoryservices-organization.md).|
|[Update organization](../api/microsoft.directoryservices-organization-update.md)|[organization](../resources/microsoft.directoryservices-organization.md)|Update the properties of a [organization](../resources/microsoft.directoryservices-organization.md) object.|
|[checkMemberGroups](../api/microsoft.directoryservices-organization-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/microsoft.directoryservices-organization-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/microsoft.directoryservices-organization-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/microsoft.directoryservices-organization-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/microsoft.directoryservices-organization-restore.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|**TODO: Add Description**|
|[List brandings](../api/microsoft.directoryservices-organization-list-brandings.md)|[organizationalBranding](../resources/microsoft.directoryservices-organizationalbranding.md) collection|Get the organizationalBrandings from the brandings navigation property.|
|[Create brandings](../api/microsoft.directoryservices-organization-post-brandings.md)|[organizationalBranding](../resources/microsoft.directoryservices-organizationalbranding.md)|Create a new brandings object.|
|[Delete brandings](../api/microsoft.directoryservices-organization-delete-brandings.md)|None|Delete a brandings object.|
|[Update brandings](../api/microsoft.directoryservices-organization-update-brandings.md)|[organizationalBranding](../resources/microsoft.directoryservices-organizationalbranding.md)|Update the properties of a brandings object.|
|[Get organizationalBranding](../api/microsoft.directoryservices-organizationalbranding-get.md)|[organizationalBranding](../resources/microsoft.directoryservices-organizationalbranding.md)|Read properties and relationships of an [organizationalBranding](../resources/microsoft.directoryservices-organizationalbranding.md) object.|
|[List certificateBasedAuthConfiguration](../api/microsoft.directoryservices-organization-list-certificatebasedauthconfiguration.md)|[certificateBasedAuthConfiguration](../resources/microsoft.directoryservices-certificatebasedauthconfiguration.md) collection|Get the certificateBasedAuthConfigurations from the certificateBasedAuthConfiguration navigation property.|
|[Add certificateBasedAuthConfiguration](../api/microsoft.directoryservices-organization-post-certificatebasedauthconfiguration.md)|[certificateBasedAuthConfiguration](../resources/microsoft.directoryservices-certificatebasedauthconfiguration.md)|Add certificateBasedAuthConfiguration by posting to the certificateBasedAuthConfiguration collection.|
|[Remove certificateBasedAuthConfiguration](../api/microsoft.directoryservices-organization-delete-certificatebasedauthconfiguration.md)|None|Remove a certificateBasedAuthConfiguration object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedPlans|[assignedPlan](../resources/microsoft.directoryservices-assignedplan.md) collection|**TODO: Add Description**|
|businessPhones|String collection|**TODO: Add Description**|
|city|String|**TODO: Add Description**|
|country|String|**TODO: Add Description**|
|countryLetterCode|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|directorySizeQuota|[directorySizeQuota](../resources/microsoft.directoryservices-directorysizequota.md)|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|isMultipleDataLocationsForServicesEnabled|Boolean|**TODO: Add Description**|
|marketingNotificationEmails|String collection|**TODO: Add Description**|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description**|
|postalCode|String|**TODO: Add Description**|
|preferredLanguage|String|**TODO: Add Description**|
|privacyProfile|[privacyProfile](../resources/microsoft.directoryservices-privacyprofile.md)|**TODO: Add Description**|
|provisionedPlans|[provisionedPlan](../resources/microsoft.directoryservices-provisionedplan.md) collection|**TODO: Add Description**|
|securityComplianceNotificationMails|String collection|**TODO: Add Description**|
|securityComplianceNotificationPhones|String collection|**TODO: Add Description**|
|state|String|**TODO: Add Description**|
|street|String|**TODO: Add Description**|
|technicalNotificationMails|String collection|**TODO: Add Description**|
|verifiedDomains|[verifiedDomain](../resources/microsoft.directoryservices-verifieddomain.md) collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|brandings|[organizationalBranding](../resources/microsoft.directoryservices-organizationalbranding.md) collection|**TODO: Add Description**|
|certificateBasedAuthConfiguration|[certificateBasedAuthConfiguration](../resources/microsoft.directoryservices-certificatebasedauthconfiguration.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.organization",
  "baseType": "Microsoft.DirectoryServices.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.organization",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "assignedPlans": [
    {
      "@odata.type": "Microsoft.DirectoryServices.assignedPlan",
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
    "@odata.type": "Microsoft.DirectoryServices.directorySizeQuota",
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
    "@odata.type": "Microsoft.DirectoryServices.privacyProfile",
    "contactEmail": "String",
    "statementUrl": "String"
  },
  "provisionedPlans": [
    {
      "@odata.type": "Microsoft.DirectoryServices.provisionedPlan",
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
      "@odata.type": "Microsoft.DirectoryServices.verifiedDomain",
      "capabilities": "String",
      "isDefault": true,
      "isInitial": true,
      "name": "String",
      "type": "String"
    }
  ]
}
```

