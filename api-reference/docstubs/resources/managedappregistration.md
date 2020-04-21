---
title: "managedAppRegistration resource type"
description: "The ManagedAppEntity is the base entity type for all other entity types under app management workflow.
The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# managedAppRegistration resource type


Namespace: microsoft.graph

The ManagedAppEntity is the base entity type for all other entity types under app management workflow.
The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedAppRegistration](../api/managedappregistration-get.md)|[managedAppRegistration](../resources/managedappregistration.md)|Read properties and relationships of a [managedAppRegistration](../resources/managedappregistration.md) object.|
|[getUserIdsWithFlaggedAppRegistration](../api/managedappregistration-getuseridswithflaggedappregistration.md)|String collection|**TODO: Add Description**|
|[List appliedPolicies](../api/managedappregistration-list-appliedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md) collection|Get the managedAppPolicies from the appliedPolicies navigation property.|
|[Create appliedPolicies](../api/managedappregistration-post-appliedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Create a new appliedPolicies object.|
|[Delete appliedPolicies](../api/managedappregistration-delete-appliedpolicies.md)|None|Delete an appliedPolicies object.|
|[Update appliedPolicies](../api/managedappregistration-update-appliedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Update the properties of an appliedPolicies object.|
|[Get managedAppPolicy](../api/managedapppolicy-get.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Read properties and relationships of a [managedAppPolicy](../resources/managedapppolicy.md) object.|
|[List intendedPolicies](../api/managedappregistration-list-intendedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md) collection|Get the managedAppPolicies from the intendedPolicies navigation property.|
|[Create intendedPolicies](../api/managedappregistration-post-intendedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Create a new intendedPolicies object.|
|[Delete intendedPolicies](../api/managedappregistration-delete-intendedpolicies.md)|None|Delete an intendedPolicies object.|
|[Update intendedPolicies](../api/managedappregistration-update-intendedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Update the properties of an intendedPolicies object.|
|[Get managedAppPolicy](../api/managedapppolicy-get.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Read properties and relationships of a [managedAppPolicy](../resources/managedapppolicy.md) object.|
|[List operations](../api/managedappregistration-list-operations.md)|[managedAppOperation](../resources/managedappoperation.md) collection|Get the managedAppOperations from the operations navigation property.|
|[Create operations](../api/managedappregistration-post-operations.md)|[managedAppOperation](../resources/managedappoperation.md)|Create a new operations object.|
|[Delete operations](../api/managedappregistration-delete-operations.md)|None|Delete an operations object.|
|[Update operations](../api/managedappregistration-update-operations.md)|[managedAppOperation](../resources/managedappoperation.md)|Update the properties of an operations object.|
|[Get managedAppOperation](../api/managedappoperation-get.md)|[managedAppOperation](../resources/managedappoperation.md)|Read properties and relationships of a [managedAppOperation](../resources/managedappoperation.md) object.|
|[List managedAppRegistrations](../api/user-list-managedappregistrations.md)|[managedAppRegistration](../resources/managedappregistration.md) collection|Get the managedAppRegistrations from the managedAppRegistrations navigation property.|
|[Add managedAppRegistrations](../api/user-post-managedappregistrations.md)|[managedAppRegistration](../resources/managedappregistration.md)|Add managedAppRegistrations by posting to the managedAppRegistrations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appIdentifier|[mobileAppIdentifier](../resources/mobileappidentifier.md)|The app package Identifier|
|applicationVersion|String|App version|
|createdDateTime|DateTimeOffset|Date and time of creation|
|deviceName|String|Host device name|
|deviceTag|String|App management SDK generated tag, which helps relate apps hosted on the same device. Not guaranteed to relate apps in all conditions.|
|deviceType|String|Host device type|
|flaggedReasons|managedAppFlaggedReason collection|Zero or more reasons an app registration is flagged. E.g. app running on rooted device|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset|Date and time of last the app synced with management service.|
|managementSdkVersion|String|App management SDK version|
|platformVersion|String|Operating System version|
|userId|String|The user Id to who this app registration belongs.|
|version|String|Version of the entity.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliedPolicies|[managedAppPolicy](../resources/managedapppolicy.md) collection|Zero or more policys already applied on the registered app when it last synchronized with managment service.|
|intendedPolicies|[managedAppPolicy](../resources/managedapppolicy.md) collection|Zero or more policies admin intended for the app as of now.|
|operations|[managedAppOperation](../resources/managedappoperation.md) collection|Zero or more long running operations triggered on the app registration.|

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

