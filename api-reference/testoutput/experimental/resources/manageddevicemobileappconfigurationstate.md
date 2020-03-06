---
title: "managedDeviceMobileAppConfigurationState resource type"
description: "Managed Device Mobile App Configuration State for a given device."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedDeviceMobileAppConfigurationState resource type


Namespace: microsoft.graph

Managed Device Mobile App Configuration State for a given device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedDeviceMobileAppConfigurationState](../api/manageddevicemobileappconfigurationstate-get.md)|[managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md)|Read properties and relationships of the [managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md) object.|
|[Update managedDeviceMobileAppConfigurationState](../api/manageddevicemobileappconfigurationstate-update.md)|[managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md)|Update the properties of a [managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md) object.|
|[List managedDeviceMobileAppConfigurationStates](../api/manageddevice-list-manageddevicemobileappconfigurationstates.md)|[managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md) collection|Get the managedDeviceMobileAppConfigurationStates from the managedDeviceMobileAppConfigurationStates navigation property.|
|[Add managedDeviceMobileAppConfigurationStates](../api/manageddevice-post-manageddevicemobileappconfigurationstates.md)|[managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md)|Add managedDeviceMobileAppConfigurationStates by posting to the managedDeviceMobileAppConfigurationStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The name of the policy for this policyBase|
|id|String| Inherited from [entity](../resources/entity.md)|
|platformType|Enumeration|Platform type that the policy applies to. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|settingCount|Int32|Count of how many setting a policy holds|
|state|Enumeration|The compliance state of the policy. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|userId|String|User unique identifier, must be Guid|
|userPrincipalName|String|User Principal Name|
|version|Int32|The version of the policy|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationState",
  "id": "String (identifier)",
  "displayName": "String",
  "version": 1024,
  "platformType": "String",
  "state": "String",
  "settingCount": 1024,
  "userId": "String",
  "userPrincipalName": "String"
}
```

