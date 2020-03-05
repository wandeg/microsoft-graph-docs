---
title: "deviceConfigurationDeviceStatus resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceConfigurationDeviceStatus resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceConfigurationDeviceStatuses](../api/deviceconfigurationdevicestatus-list.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) objects.|
|[Get deviceConfigurationDeviceStatus](../api/deviceconfigurationdevicestatus-get.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Read properties and relationships of the [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) object.|
|[Create deviceConfigurationDeviceStatus](../api/deviceconfigurationdevicestatus-create.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Create a new [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) object.|
|[Delete deviceConfigurationDeviceStatus](../api/deviceconfigurationdevicestatus-delete.md)|None|Deletes a [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md).|
|[Update deviceConfigurationDeviceStatus](../api/deviceconfigurationdevicestatus-update.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Update the properties of a [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|The DateTime when device compliance grace period expires|
|deviceDisplayName|String|Device name of the DevicePolicyStatus.|
|deviceModel|String|The device model that is being reported|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastReportedDateTime|DateTimeOffset|Last modified date time of the policy report.|
|status|Enumeration|Compliance status of the policy report. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|userName|String|The User Name that is being reported|
|userPrincipalName|String|UserPrincipalName.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```

