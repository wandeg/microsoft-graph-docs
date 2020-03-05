---
title: "androidManagedAppRegistration resource type"
description: "Represents the synchronization details of an android app, with management capabilities, for a specific user.
The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# androidManagedAppRegistration resource type


Namespace: microsoft.graph

Represents the synchronization details of an android app, with management capabilities, for a specific user.
The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.


Inherits from [managedAppRegistration](../resources/managedappregistration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List androidManagedAppRegistrations](../api/androidmanagedappregistration-list.md)|[androidManagedAppRegistration](../resources/androidmanagedappregistration.md) collection|List properties and relationships of the [androidManagedAppRegistration](../resources/androidmanagedappregistration.md) objects.|
|[Get androidManagedAppRegistration](../api/androidmanagedappregistration-get.md)|[androidManagedAppRegistration](../resources/androidmanagedappregistration.md)|Read properties and relationships of the [androidManagedAppRegistration](../resources/androidmanagedappregistration.md) object.|
|[Create androidManagedAppRegistration](../api/androidmanagedappregistration-create.md)|[androidManagedAppRegistration](../resources/androidmanagedappregistration.md)|Create a new [androidManagedAppRegistration](../resources/androidmanagedappregistration.md) object.|
|[Delete androidManagedAppRegistration](../api/androidmanagedappregistration-delete.md)|None|Deletes a [androidManagedAppRegistration](../resources/androidmanagedappregistration.md).|
|[Update androidManagedAppRegistration](../api/androidmanagedappregistration-update.md)|[androidManagedAppRegistration](../resources/androidmanagedappregistration.md)|Update the properties of a [androidManagedAppRegistration](../resources/androidmanagedappregistration.md) object.|
|[List appliedPolicies](../api/androidmanagedappregistration-list-appliedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md) collection|Get the managedAppPolicies from the appliedPolicies navigation property.|
|[Add appliedPolicies](../api/androidmanagedappregistration-post-appliedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Add appliedPolicies by posting to the appliedPolicies collection.|
|[List intendedPolicies](../api/androidmanagedappregistration-list-intendedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md) collection|Get the managedAppPolicies from the intendedPolicies navigation property.|
|[Add intendedPolicies](../api/androidmanagedappregistration-post-intendedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Add intendedPolicies by posting to the intendedPolicies collection.|
|[List operations](../api/androidmanagedappregistration-list-operations.md)|[managedAppOperation](../resources/managedappoperation.md) collection|Get the managedAppOperations from the operations navigation property.|
|[Add operations](../api/androidmanagedappregistration-post-operations.md)|[managedAppOperation](../resources/managedappoperation.md)|Add operations by posting to the operations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appIdentifier|[mobileAppIdentifier](../resources/mobileappidentifier.md)|The app package Identifier Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|applicationVersion|String|App version Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|createdDateTime|DateTimeOffset|Date and time of creation Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|deviceName|String|Host device name Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|deviceTag|String|App management SDK generated tag, which helps relate apps hosted on the same device. Not guaranteed to relate apps in all conditions. Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|deviceType|String|Host device type Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|flaggedReasons|Enumeration collection|Zero or more reasons an app registration is flagged. E.g. app running on rooted device Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset|Date and time of last the app synced with management service. Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|managementSdkVersion|String|App management SDK version Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|platformVersion|String|Operating System version Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|userId|String|The user Id to who this app registration belongs. Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|version|String|Version of the entity. Inherited from [managedAppRegistration](../resources/managedappregistration.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliedPolicies|[managedAppPolicy](../resources/managedapppolicy.md) collection|Zero or more policys already applied on the registered app when it last synchronized with managment service. Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|intendedPolicies|[managedAppPolicy](../resources/managedapppolicy.md) collection|Zero or more policies admin intended for the app as of now. Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|operations|[managedAppOperation](../resources/managedappoperation.md) collection|Zero or more long running operations triggered on the app registration. Inherited from [managedAppRegistration](../resources/managedappregistration.md)|

## JSON representation
Here is a JSON representation of the resource.
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

