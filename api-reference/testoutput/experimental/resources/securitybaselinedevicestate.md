---
title: "securityBaselineDeviceState resource type"
description: "The security baseline compliance state summary of the security baseline for a device."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# securityBaselineDeviceState resource type


Namespace: microsoft.graph

The security baseline compliance state summary of the security baseline for a device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List securityBaselineDeviceStates](../api/securitybaselinedevicestate-list.md)|[securityBaselineDeviceState](../resources/securitybaselinedevicestate.md) collection|List properties and relationships of the [securityBaselineDeviceState](../resources/securitybaselinedevicestate.md) objects.|
|[Get securityBaselineDeviceState](../api/securitybaselinedevicestate-get.md)|[securityBaselineDeviceState](../resources/securitybaselinedevicestate.md)|Read properties and relationships of the [securityBaselineDeviceState](../resources/securitybaselinedevicestate.md) object.|
|[Create securityBaselineDeviceState](../api/securitybaselinedevicestate-create.md)|[securityBaselineDeviceState](../resources/securitybaselinedevicestate.md)|Create a new [securityBaselineDeviceState](../resources/securitybaselinedevicestate.md) object.|
|[Delete securityBaselineDeviceState](../api/securitybaselinedevicestate-delete.md)|None|Deletes a [securityBaselineDeviceState](../resources/securitybaselinedevicestate.md).|
|[Update securityBaselineDeviceState](../api/securitybaselinedevicestate-update.md)|[securityBaselineDeviceState](../resources/securitybaselinedevicestate.md)|Update the properties of a [securityBaselineDeviceState](../resources/securitybaselinedevicestate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceDisplayName|String|Display name of the device|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastReportedDateTime|DateTimeOffset|Last modified date time of the policy report|
|managedDeviceId|String|Intune device id|
|state|Enumeration|Security baseline compliance state. Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.|
|userPrincipalName|String|User Principal Name|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineDeviceState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
  "id": "String (identifier)",
  "managedDeviceId": "String",
  "deviceDisplayName": "String",
  "userPrincipalName": "String",
  "state": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```

