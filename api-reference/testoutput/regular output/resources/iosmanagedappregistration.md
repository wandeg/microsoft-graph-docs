---
title: "iosManagedAppRegistration resource type"
description: "Represents the synchronization details of an ios app, with management capabilities, for a specific user.
The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# iosManagedAppRegistration resource type

Represents the synchronization details of an ios app, with management capabilities, for a specific user.
The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.


Inherits from [managedAppRegistration](../resources/managedAppRegistration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List iosManagedAppRegistrations](../api/iosmanagedappregistration-list.md)|[iosManagedAppRegistration](../resources/iosManagedAppRegistration.md) collection|List properties and relationships of the [iosManagedAppRegistration](../resources/iosmanagedappregistration.md) objects.|
|[Get iosManagedAppRegistration](../api/iosmanagedappregistration-get.md)|[iosManagedAppRegistration](../resources/iosManagedAppRegistration.md)|Read properties and relationships of the [iosManagedAppRegistration](../resources/iosmanagedappregistration.md) object.|
|[Create iosManagedAppRegistration](../api/iosmanagedappregistration-create.md)|[iosManagedAppRegistration](../resources/iosManagedAppRegistration.md)|Create a new [iosManagedAppRegistration](../resources/iosmanagedappregistration.md) object.|
|[Delete iosManagedAppRegistration](../api/iosmanagedappregistration-delete.md)|None|Deletes a [iosManagedAppRegistration](../resources/iosmanagedappregistration.md).|
|[Update iosManagedAppRegistration](../api/iosmanagedappregistration-update.md)|[iosManagedAppRegistration](../resources/iosManagedAppRegistration.md)|Update the properties of a [iosManagedAppRegistration](../resources/iosmanagedappregistration.md) object.|
|[List appliedPolicies](../api/iosmanagedappregistration-list-appliedpolicies.md)|[managedAppPolicy](../resources/managedAppPolicy.md) collection|Get the managedAppPolicies from the appliedPolicies navigation property.|
|[Add appliedPolicies](../api/iosmanagedappregistration-post-appliedpolicies.md)|[managedAppPolicy](../resources/managedAppPolicy.md)|Add appliedPolicies by posting to the appliedPolicies collection.|
|[List intendedPolicies](../api/iosmanagedappregistration-list-intendedpolicies.md)|[managedAppPolicy](../resources/managedAppPolicy.md) collection|Get the managedAppPolicies from the intendedPolicies navigation property.|
|[Add intendedPolicies](../api/iosmanagedappregistration-post-intendedpolicies.md)|[managedAppPolicy](../resources/managedAppPolicy.md)|Add intendedPolicies by posting to the intendedPolicies collection.|
|[List operations](../api/iosmanagedappregistration-list-operations.md)|[managedAppOperation](../resources/managedAppOperation.md) collection|Get the managedAppOperations from the operations navigation property.|
|[Add operations](../api/iosmanagedappregistration-post-operations.md)|[managedAppOperation](../resources/managedAppOperation.md)|Add operations by posting to the operations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appIdentifier|[mobileAppIdentifier](../resources/mobileAppIdentifier.md)|The app package Identifier Inherited from [managedAppRegistration](../resources/managedAppRegistration.md)|
|applicationVersion|String|App version Inherited from [managedAppRegistration](../resources/managedAppRegistration.md)|
|createdDateTime|DateTimeOffset|Date and time of creation Inherited from [managedAppRegistration](../resources/managedAppRegistration.md)|
|deviceName|String|Host device name Inherited from [managedAppRegistration](../resources/managedAppRegistration.md)|
|deviceTag|String|App management SDK generated tag, which helps relate apps hosted on the same device. Not guaranteed to relate apps in all conditions. Inherited from [managedAppRegistration](../resources/managedAppRegistration.md)|
|deviceType|String|Host device type Inherited from [managedAppRegistration](../resources/managedAppRegistration.md)|
|flaggedReasons|Enumeration collection|Zero or more reasons an app registration is flagged. E.g. app running on rooted device Inherited from [managedAppRegistration](../resources/managedAppRegistration.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset|Date and time of last the app synced with management service. Inherited from [managedAppRegistration](../resources/managedAppRegistration.md)|
|managementSdkVersion|String|App management SDK version Inherited from [managedAppRegistration](../resources/managedAppRegistration.md)|
|platformVersion|String|Operating System version Inherited from [managedAppRegistration](../resources/managedAppRegistration.md)|
|userId|String|The user Id to who this app registration belongs. Inherited from [managedAppRegistration](../resources/managedAppRegistration.md)|
|version|String|Version of the entity. Inherited from [managedAppRegistration](../resources/managedAppRegistration.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliedPolicies|[managedAppPolicy](../resources/managedAppPolicy.md) collection|Zero or more policys already applied on the registered app when it last synchronized with managment service. Inherited from [managedAppRegistration](../resources/managedAppRegistration.md)|
|intendedPolicies|[managedAppPolicy](../resources/managedAppPolicy.md) collection|Zero or more policies admin intended for the app as of now. Inherited from [managedAppRegistration](../resources/managedAppRegistration.md)|
|operations|[managedAppOperation](../resources/managedAppOperation.md) collection|Zero or more long running operations triggered on the app registration. Inherited from [managedAppRegistration](../resources/managedAppRegistration.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosManagedAppRegistration",
  "baseType": "microsoft.graph.managedAppRegistration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
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

