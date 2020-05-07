---
title: "windowsInformationProtectionDeviceRegistration resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsInformationProtectionDeviceRegistration resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[wipe](../api/windowsinformationprotectiondeviceregistration-wipe.md)|None|**TODO: Add Description**|
|[List windowsInformationProtectionDeviceRegistrations](../api/user-list-windowsinformationprotectiondeviceregistrations.md)|[windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md) collection|Get the windowsInformationProtectionDeviceRegistrations from the windowsInformationProtectionDeviceRegistrations navigation property.|
|[Add windowsInformationProtectionDeviceRegistrations](../api/user-post-windowsinformationprotectiondeviceregistrations.md)|[windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md)|Add windowsInformationProtectionDeviceRegistrations by posting to the windowsInformationProtectionDeviceRegistrations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceMacAddress|String|**TODO: Add Description**|
|deviceName|String|**TODO: Add Description**|
|deviceRegistrationId|String|**TODO: Add Description**|
|deviceType|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastCheckInDateTime|DateTimeOffset|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "id": "String (identifier)",
  "userId": "String",
  "deviceRegistrationId": "String",
  "deviceName": "String",
  "deviceType": "String",
  "deviceMacAddress": "String",
  "lastCheckInDateTime": "String (timestamp)"
}
```

