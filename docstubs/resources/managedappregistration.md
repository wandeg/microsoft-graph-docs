---
title: "managedAppRegistration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedAppRegistration resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedAppRegistration](../api/managedappregistration-get.md)|[managedAppRegistration](../resources/managedappregistration.md)|Read properties and relationships of the [managedAppRegistration](../resources/managedappregistration.md) object.|
|[getUserIdsWithFlaggedAppRegistration](../api/managedappregistration-getuseridswithflaggedappregistration.md)|String collection||
|[List appliedPolicies](../api/managedappregistration-list-appliedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md) collection|Get the managedAppPolicies from the appliedPolicies navigation property.|
|[Add appliedPolicies](../api/managedappregistration-post-appliedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Add appliedPolicies by posting to the appliedPolicies collection.|
|[List intendedPolicies](../api/managedappregistration-list-intendedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md) collection|Get the managedAppPolicies from the intendedPolicies navigation property.|
|[Add intendedPolicies](../api/managedappregistration-post-intendedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Add intendedPolicies by posting to the intendedPolicies collection.|
|[List operations](../api/managedappregistration-list-operations.md)|[managedAppOperation](../resources/managedappoperation.md) collection|Get the managedAppOperations from the operations navigation property.|
|[Add operations](../api/managedappregistration-post-operations.md)|[managedAppOperation](../resources/managedappoperation.md)|Add operations by posting to the operations collection.|
|[List managedAppRegistrations](../api/user-list-managedappregistrations.md)|[managedAppRegistration](../resources/managedappregistration.md) collection|Get the managedAppRegistrations from the managedAppRegistrations navigation property.|
|[Create managedAppRegistrations](../api/user-post-managedappregistrations.md)|[managedAppRegistration](../resources/managedappregistration.md)|Create managedAppRegistrations by posting to the managedAppRegistrations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appIdentifier|[mobileAppIdentifier](../resources/mobileappidentifier.md)||
|applicationVersion|String||
|azureADDeviceId|String||
|createdDateTime|DateTimeOffset||
|deviceManufacturer|String||
|deviceModel|String||
|deviceName|String||
|deviceTag|String||
|deviceType|String||
|flaggedReasons|Enumeration collection||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset||
|managedDeviceId|String||
|managementSdkVersion|String||
|platformVersion|String||
|userId|String||
|version|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliedPolicies|[managedAppPolicy](../resources/managedapppolicy.md) collection||
|intendedPolicies|[managedAppPolicy](../resources/managedapppolicy.md) collection||
|operations|[managedAppOperation](../resources/managedappoperation.md) collection||

## JSON representation
Here is a JSON representation of the resource.
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

