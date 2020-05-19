---
title: "managedAppRegistration resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedAppRegistration resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managedAppRegistrations](../api/user-list-managedappregistrations.md)|[managedAppRegistration](../resources/intune-managedappregistration.md) collection|Get the managedAppRegistrations from the managedAppRegistrations navigation property.|
|[Add managedAppRegistrations](../api/user-post-managedappregistrations.md)|[managedAppRegistration](../resources/intune-managedappregistration.md)|Add managedAppRegistrations by posting to the managedAppRegistrations collection.|
|[Remove managedAppRegistrations](../api/user-delete-managedappregistrations.md)|None|Remove a [managedAppRegistration](../resources/intune-managedappregistration.md) object.|
|[getUserIdsWithFlaggedAppRegistration](../api/intune-managedappregistration-getuseridswithflaggedappregistration.md)|String collection|**TODO: Add Description**|
|[List appliedPolicies](../api/intune-managedappregistration-list-appliedpolicies.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md) collection|Get the managedAppPolicies from the appliedPolicies navigation property.|
|[Create appliedPolicies](../api/intune-managedappregistration-post-appliedpolicies.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md)|Create a new appliedPolicies object.|
|[Delete appliedPolicies](../api/intune-managedappregistration-delete-appliedpolicies.md)|None|Delete a [managedAppPolicy](../resources/intune-managedapppolicy.md) object.|
|[Update appliedPolicies](../api/intune-managedappregistration-update-appliedpolicies.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md)|Update the properties of an appliedPolicies object.|
|[Get appliedPolicies](../api/intune-managedappregistration-get-managedapppolicy.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md)|Read the properties and relationships of a [managedAppPolicy](../resources/intune-managedapppolicy.md) object.|
|[List intendedPolicies](../api/intune-managedappregistration-list-intendedpolicies.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md) collection|Get the managedAppPolicies from the intendedPolicies navigation property.|
|[Create intendedPolicies](../api/intune-managedappregistration-post-intendedpolicies.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md)|Create a new intendedPolicies object.|
|[Delete intendedPolicies](../api/intune-managedappregistration-delete-intendedpolicies.md)|None|Delete a [managedAppPolicy](../resources/intune-managedapppolicy.md) object.|
|[Update intendedPolicies](../api/intune-managedappregistration-update-intendedpolicies.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md)|Update the properties of an intendedPolicies object.|
|[Get intendedPolicies](../api/intune-managedappregistration-get-managedapppolicy.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md)|Read the properties and relationships of a [managedAppPolicy](../resources/intune-managedapppolicy.md) object.|
|[List operations](../api/intune-managedappregistration-list-operations.md)|[managedAppOperation](../resources/intune-managedappoperation.md) collection|Get the managedAppOperations from the operations navigation property.|
|[Create operations](../api/intune-managedappregistration-post-operations.md)|[managedAppOperation](../resources/intune-managedappoperation.md)|Create a new operations object.|
|[Delete operations](../api/intune-managedappregistration-delete-operations.md)|None|Delete a [managedAppOperation](../resources/intune-managedappoperation.md) object.|
|[Update operations](../api/intune-managedappregistration-update-operations.md)|[managedAppOperation](../resources/intune-managedappoperation.md)|Update the properties of an operations object.|
|[Get operations](../api/intune-managedappregistration-get-managedappoperation.md)|[managedAppOperation](../resources/intune-managedappoperation.md)|Read the properties and relationships of a [managedAppOperation](../resources/intune-managedappoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mobileappidentifier.md)|**TODO: Add Description**|
|applicationVersion|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|deviceName|String|**TODO: Add Description**|
|deviceTag|String|**TODO: Add Description**|
|deviceType|String|**TODO: Add Description**|
|flaggedReasons|managedAppFlaggedReason collection|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|managementSdkVersion|String|**TODO: Add Description**|
|platformVersion|String|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|version|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliedPolicies|[managedAppPolicy](../resources/intune-managedapppolicy.md) collection|**TODO: Add Description**|
|intendedPolicies|[managedAppPolicy](../resources/intune-managedapppolicy.md) collection|**TODO: Add Description**|
|operations|[managedAppOperation](../resources/intune-managedappoperation.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppRegistration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "String"
}
```

