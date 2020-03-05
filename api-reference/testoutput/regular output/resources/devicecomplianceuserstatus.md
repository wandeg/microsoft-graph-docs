---
title: "deviceComplianceUserStatus resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceComplianceUserStatus resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceComplianceUserStatuses](../api/devicecomplianceuserstatus-list.md)|[deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md) collection|List properties and relationships of the [deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md) objects.|
|[Get deviceComplianceUserStatus](../api/devicecomplianceuserstatus-get.md)|[deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md)|Read properties and relationships of the [deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md) object.|
|[Create deviceComplianceUserStatus](../api/devicecomplianceuserstatus-create.md)|[deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md)|Create a new [deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md) object.|
|[Delete deviceComplianceUserStatus](../api/devicecomplianceuserstatus-delete.md)|None|Deletes a [deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md).|
|[Update deviceComplianceUserStatus](../api/devicecomplianceuserstatus-update.md)|[deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md)|Update the properties of a [deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|devicesCount|Int32|Devices count for that user.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastReportedDateTime|DateTimeOffset|Last modified date time of the policy report.|
|status|Enumeration|Compliance status of the policy report. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|userDisplayName|String|User name of the DevicePolicyStatus.|
|userPrincipalName|String|UserPrincipalName.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceUserStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "devicesCount": 1024,
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```

