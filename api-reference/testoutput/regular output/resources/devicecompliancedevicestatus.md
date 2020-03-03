---
title: "deviceComplianceDeviceStatus resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceComplianceDeviceStatus resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceComplianceDeviceStatus](../api/devicecompliancedevicestatus-get.md)|[deviceComplianceDeviceStatus](../resources/deviceComplianceDeviceStatus.md)|Read properties and relationships of the [deviceComplianceDeviceStatus](../resources/devicecompliancedevicestatus.md) object.|
|[Delete deviceComplianceDeviceStatus](../api/devicecompliancedevicestatus-delete.md)|None|Deletes a [deviceComplianceDeviceStatus](../resources/devicecompliancedevicestatus.md).|
|[Update deviceComplianceDeviceStatus](../api/devicecompliancedevicestatus-update.md)|[deviceComplianceDeviceStatus](../resources/deviceComplianceDeviceStatus.md)|Update the properties of a [deviceComplianceDeviceStatus](../resources/devicecompliancedevicestatus.md) object.|

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

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceDeviceStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
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

