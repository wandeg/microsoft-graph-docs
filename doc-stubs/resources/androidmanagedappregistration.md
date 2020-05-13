---
title: "androidManagedAppRegistration resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# androidManagedAppRegistration resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [managedAppRegistration](../resources/managedappregistration.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List appliedPolicies](../api/androidmanagedappregistration-list-appliedpolicies.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md) collection|Get the managedAppPolicies from the appliedPolicies navigation property.|
|[Create appliedPolicies](../api/androidmanagedappregistration-post-appliedpolicies.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md)|Create a new appliedPolicies object.|
|[Delete appliedPolicies](../api/androidmanagedappregistration-delete-appliedpolicies.md)|None|Delete a [managedAppPolicy](../resources/intune-managedapppolicy.md) object.|
|[Update appliedPolicies](../api/androidmanagedappregistration-update-appliedpolicies.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md)|Update the properties of an appliedPolicies object.|
|[Get appliedPolicies](../api/androidmanagedappregistration-get-managedapppolicy.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md)|Read the properties and relationships of a [managedAppPolicy](../resources/intune-managedapppolicy.md) object.|
|[List intendedPolicies](../api/androidmanagedappregistration-list-intendedpolicies.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md) collection|Get the managedAppPolicies from the intendedPolicies navigation property.|
|[Create intendedPolicies](../api/androidmanagedappregistration-post-intendedpolicies.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md)|Create a new intendedPolicies object.|
|[Delete intendedPolicies](../api/androidmanagedappregistration-delete-intendedpolicies.md)|None|Delete a [managedAppPolicy](../resources/intune-managedapppolicy.md) object.|
|[Update intendedPolicies](../api/androidmanagedappregistration-update-intendedpolicies.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md)|Update the properties of an intendedPolicies object.|
|[Get intendedPolicies](../api/androidmanagedappregistration-get-managedapppolicy.md)|[managedAppPolicy](../resources/intune-managedapppolicy.md)|Read the properties and relationships of a [managedAppPolicy](../resources/intune-managedapppolicy.md) object.|
|[List operations](../api/androidmanagedappregistration-list-operations.md)|[managedAppOperation](../resources/intune-managedappoperation.md) collection|Get the managedAppOperations from the operations navigation property.|
|[Create operations](../api/androidmanagedappregistration-post-operations.md)|[managedAppOperation](../resources/intune-managedappoperation.md)|Create a new operations object.|
|[Delete operations](../api/androidmanagedappregistration-delete-operations.md)|None|Delete a [managedAppOperation](../resources/intune-managedappoperation.md) object.|
|[Update operations](../api/androidmanagedappregistration-update-operations.md)|[managedAppOperation](../resources/intune-managedappoperation.md)|Update the properties of an operations object.|
|[Get operations](../api/androidmanagedappregistration-get-managedappoperation.md)|[managedAppOperation](../resources/intune-managedappoperation.md)|Read the properties and relationships of a [managedAppOperation](../resources/intune-managedappoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mobileappidentifier.md)|**TODO: Add Description** Inherited from [managedAppRegistration](../resources/intune-managedappregistration.md)|
|applicationVersion|String|**TODO: Add Description** Inherited from [managedAppRegistration](../resources/intune-managedappregistration.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedAppRegistration](../resources/intune-managedappregistration.md)|
|deviceName|String|**TODO: Add Description** Inherited from [managedAppRegistration](../resources/intune-managedappregistration.md)|
|deviceTag|String|**TODO: Add Description** Inherited from [managedAppRegistration](../resources/intune-managedappregistration.md)|
|deviceType|String|**TODO: Add Description** Inherited from [managedAppRegistration](../resources/intune-managedappregistration.md)|
|flaggedReasons|managedAppFlaggedReason collection|**TODO: Add Description** Inherited from [managedAppRegistration](../resources/intune-managedappregistration.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedAppRegistration](../resources/intune-managedappregistration.md)|
|managementSdkVersion|String|**TODO: Add Description** Inherited from [managedAppRegistration](../resources/intune-managedappregistration.md)|
|platformVersion|String|**TODO: Add Description** Inherited from [managedAppRegistration](../resources/intune-managedappregistration.md)|
|userId|String|**TODO: Add Description** Inherited from [managedAppRegistration](../resources/intune-managedappregistration.md)|
|version|String|**TODO: Add Description** Inherited from [managedAppRegistration](../resources/intune-managedappregistration.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliedPolicies|[managedAppPolicy](../resources/intune-managedapppolicy.md) collection|**TODO: Add Description** Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|intendedPolicies|[managedAppPolicy](../resources/intune-managedapppolicy.md) collection|**TODO: Add Description** Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|operations|[managedAppOperation](../resources/intune-managedappoperation.md) collection|**TODO: Add Description** Inherited from [managedAppRegistration](../resources/managedappregistration.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedAppRegistration",
  "baseType": "microsoft.graph.managedAppRegistration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
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

