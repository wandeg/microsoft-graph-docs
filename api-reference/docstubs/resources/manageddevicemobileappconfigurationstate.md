---
title: "managedDeviceMobileAppConfigurationState resource type"
description: "Managed Device Mobile App Configuration State for a given device."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedDeviceMobileAppConfigurationState resource type


Namespace: microsoft.graph

Managed Device Mobile App Configuration State for a given device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedDeviceMobileAppConfigurationState](../api/manageddevicemobileappconfigurationstate-get.md)|[managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md)|Read the properties and relationships of a [managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md) object.|
|[Update managedDeviceMobileAppConfigurationState](../api/manageddevicemobileappconfigurationstate-update.md)|[managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md)|Update the properties of a [managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The name of the policy for this policyBase|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|platformType|policyPlatformType|Platform type that the policy applies to. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.|
|settingCount|Int32|Count of how many setting a policy holds|
|settingStates|[managedDeviceMobileAppConfigurationSettingState](../resources/manageddevicemobileappconfigurationsettingstate.md) collection|**TODO: Add Description**|
|state|complianceStatus|The compliance state of the policy. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
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
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState"
    }
  ],
  "displayName": "String",
  "version": 1024,
  "platformType": "String",
  "state": "String",
  "settingCount": 1024,
  "userId": "String",
  "userPrincipalName": "String"
}
```

