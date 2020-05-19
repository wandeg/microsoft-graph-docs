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
|[List branding](../api/organization-list-branding.md)|[organizationalBranding](../resources/organizationalbranding.md) collection|Get the organizationalBrandings from the branding navigation property.|
|[Create branding](../api/organization-post-branding.md)|[organizationalBranding](../resources/organizationalbranding.md)|Create a new branding object.|
|[Delete branding](../api/organization-delete-branding.md)|None|Delete an [organizationalBranding](../resources/organizationalbranding.md) object.|
|[Update branding](../api/organization-update-branding.md)|[organizationalBranding](../resources/organizationalbranding.md)|Update the properties of a branding object.|
|[Get branding](../api/organization-get-organizationalbranding.md)|[organizationalBranding](../resources/organizationalbranding.md)|Read the properties and relationships of an [organizationalBranding](../resources/organizationalbranding.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedPlans|[assignedPlan](../resources/assignedplan.md) collection|**TODO: Add Description**|
|businessPhones|String collection|**TODO: Add Description**|
|city|String|**TODO: Add Description**|
|country|String|**TODO: Add Description**|
|countryLetterCode|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|directorySizeQuota|[directorySizeQuota](../resources/directorysizequota.md)|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|isMultipleDataLocationsForServicesEnabled|Boolean|**TODO: Add Description**|
|marketingNotificationEmails|String collection|**TODO: Add Description**|
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
|branding|[organizationalBranding](../resources/organizationalbranding.md)|**TODO: Add Description**|
|certificateBasedAuthConfiguration|[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization",
  "baseType": "Microsoft.DirectoryServices.directoryObject",
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
  ]
}
```

