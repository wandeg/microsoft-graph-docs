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
|[getUserIdsWithFlaggedAppRegistration](../api/managedappregistration-getuseridswithflaggedappregistration.md)|String collection|**TODO: Add Description**|
|[List appliedPolicies](../api/managedappregistration-list-appliedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md) collection|Get the managedAppPolicies from the appliedPolicies navigation property.|
|[Create appliedPolicies](../api/managedappregistration-post-appliedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Create a new appliedPolicies object.|
|[Delete appliedPolicies](../api/managedappregistration-delete-appliedpolicies.md)|None|Delete an [managedAppPolicy](../resources/managedapppolicy.md) object.|
|[Update appliedPolicies](../api/managedappregistration-update-appliedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Update the properties of an appliedPolicies object.|
|[Get managedAppPolicy](../api/managedapppolicy-get.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Read the properties and relationships of a [managedAppPolicy](../resources/managedapppolicy.md) object.|
|[List intendedPolicies](../api/managedappregistration-list-intendedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md) collection|Get the managedAppPolicies from the intendedPolicies navigation property.|
|[Create intendedPolicies](../api/managedappregistration-post-intendedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Create a new intendedPolicies object.|
|[Delete intendedPolicies](../api/managedappregistration-delete-intendedpolicies.md)|None|Delete an [managedAppPolicy](../resources/managedapppolicy.md) object.|
|[Update intendedPolicies](../api/managedappregistration-update-intendedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Update the properties of an intendedPolicies object.|
|[Get managedAppPolicy](../api/managedapppolicy-get.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Read the properties and relationships of a [managedAppPolicy](../resources/managedapppolicy.md) object.|
|[List operations](../api/managedappregistration-list-operations.md)|[managedAppOperation](../resources/managedappoperation.md) collection|Get the managedAppOperations from the operations navigation property.|
|[Create operations](../api/managedappregistration-post-operations.md)|[managedAppOperation](../resources/managedappoperation.md)|Create a new operations object.|
|[Delete operations](../api/managedappregistration-delete-operations.md)|None|Delete an [managedAppOperation](../resources/managedappoperation.md) object.|
|[Update operations](../api/managedappregistration-update-operations.md)|[managedAppOperation](../resources/managedappoperation.md)|Update the properties of an operations object.|
|[Get managedAppOperation](../api/managedappoperation-get.md)|[managedAppOperation](../resources/managedappoperation.md)|Read the properties and relationships of a [managedAppOperation](../resources/managedappoperation.md) object.|
|[List managedAppRegistrations](../api/user-list-managedappregistrations.md)|[managedAppRegistration](../resources/managedappregistration.md) collection|Get the managedAppRegistrations from the managedAppRegistrations navigation property.|
|[Add managedAppRegistrations](../api/user-post-managedappregistrations.md)|[managedAppRegistration](../resources/managedappregistration.md)|Add managedAppRegistrations by posting to the managedAppRegistrations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appIdentifier|[mobileAppIdentifier](../resources/mobileappidentifier.md)|**TODO: Add Description**|
|applicationVersion|String|**TODO: Add Description**|
|azureADDeviceId|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|deviceManufacturer|String|**TODO: Add Description**|
|deviceModel|String|**TODO: Add Description**|
|deviceName|String|**TODO: Add Description**|
|deviceTag|String|**TODO: Add Description**|
|deviceType|String|**TODO: Add Description**|
|flaggedReasons|managedAppFlaggedReason collection|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|managedDeviceId|String|**TODO: Add Description**|
|managementSdkVersion|String|**TODO: Add Description**|
|platformVersion|String|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|version|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliedPolicies|[managedAppPolicy](../resources/managedapppolicy.md) collection|**TODO: Add Description**|
|intendedPolicies|[managedAppPolicy](../resources/managedapppolicy.md) collection|**TODO: Add Description**|
|operations|[managedAppOperation](../resources/managedappoperation.md) collection|**TODO: Add Description**|

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
  "managedDeviceId": "String",
  "azureADDeviceId": "String",
  "deviceModel": "String",
  "deviceManufacturer": "String",
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

