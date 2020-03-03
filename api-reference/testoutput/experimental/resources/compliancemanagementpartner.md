---
title: "complianceManagementPartner resource type"
description: "Compliance management partner for all platforms"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# complianceManagementPartner resource type


Namespace: microsoft.graph

Compliance management partner for all platforms


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List complianceManagementPartners](../api/compliancemanagementpartner-list.md)|[complianceManagementPartner](../resources/compliancemanagementpartner.md) collection|List properties and relationships of the [complianceManagementPartner](../resources/compliancemanagementpartner.md) objects.|
|[Get complianceManagementPartner](../api/compliancemanagementpartner-get.md)|[complianceManagementPartner](../resources/compliancemanagementpartner.md)|Read properties and relationships of the [complianceManagementPartner](../resources/compliancemanagementpartner.md) object.|
|[Create complianceManagementPartner](../api/compliancemanagementpartner-create.md)|[complianceManagementPartner](../resources/compliancemanagementpartner.md)|Create a new [complianceManagementPartner](../resources/compliancemanagementpartner.md) object.|
|[Delete complianceManagementPartner](../api/compliancemanagementpartner-delete.md)|None|Deletes a [complianceManagementPartner](../resources/compliancemanagementpartner.md).|
|[Update complianceManagementPartner](../api/compliancemanagementpartner-update.md)|[complianceManagementPartner](../resources/compliancemanagementpartner.md)|Update the properties of a [complianceManagementPartner](../resources/compliancemanagementpartner.md) object.|
|[List complianceManagementPartners](../api/intune-devices-devicemanagement-list-compliancemanagementpartners.md)|[complianceManagementPartner](../resources/compliancemanagementpartner.md) collection|Get the complianceManagementPartners from the complianceManagementPartners navigation property.|
|[Add complianceManagementPartners](../api/intune-devices-devicemanagement-post-compliancemanagementpartners.md)|[complianceManagementPartner](../resources/compliancemanagementpartner.md)|Add complianceManagementPartners by posting to the complianceManagementPartners collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|androidEnrollmentAssignments|[complianceManagementPartnerAssignment](../resources/compliancemanagementpartnerassignment.md) collection|User groups which enroll Android devices through partner.|
|androidOnboarded|Boolean|Partner onboarded for Android devices.|
|displayName|String|Partner display name|
|id|String| Inherited from [entity](../resources/entity.md)|
|iosEnrollmentAssignments|[complianceManagementPartnerAssignment](../resources/compliancemanagementpartnerassignment.md) collection|User groups which enroll ios devices through partner.|
|iosOnboarded|Boolean|Partner onboarded for ios devices.|
|lastHeartbeatDateTime|DateTimeOffset|Timestamp of last heartbeat after admin onboarded to the compliance management partner|
|macOsEnrollmentAssignments|[complianceManagementPartnerAssignment](../resources/compliancemanagementpartnerassignment.md) collection|User groups which enroll Mac devices through partner.|
|macOsOnboarded|Boolean|Partner onboarded for Mac devices.|
|partnerState|Enumeration|Partner state of this tenant. Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.|
|windowsEnrollmentAssignments|[complianceManagementPartnerAssignment](../resources/compliancemanagementpartnerassignment.md) collection|User groups which enroll Windows devices through partner.|
|windowsOnboarded|Boolean|Partner onboarded for Windows devices.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.complianceManagementPartner",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "displayName": "String",
  "macOsOnboarded": true,
  "windowsOnboarded": true,
  "androidOnboarded": true,
  "iosOnboarded": true,
  "macOsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
    }
  ]
}
```

