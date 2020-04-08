---
title: "deviceManagementAutopilotPolicyStatusDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementAutopilotPolicyStatusDetail resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementAutopilotPolicyStatusDetail](../api/devicemanagementautopilotpolicystatusdetail-get.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md)|Read properties and relationships of the [deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md) object.|
|[Update deviceManagementAutopilotPolicyStatusDetail](../api/devicemanagementautopilotpolicystatusdetail-update.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md)|Update the properties of a [deviceManagementAutopilotPolicyStatusDetail](../resources/devicemanagementautopilotpolicystatusdetail.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|complianceStatus|Enumeration| Possible values are: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastReportedDateTime|DateTimeOffset||
|policyType|Enumeration| Possible values are: `unknown`, `application`, `appModel`, `configurationPolicy`.|
|trackedOnEnrollmentStatus|Boolean||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "id": "String (identifier)",
  "displayName": "String",
  "policyType": "String",
  "complianceStatus": "String",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "String (timestamp)"
}
```

