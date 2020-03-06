---
title: "deviceManagementApplicabilityRuleDeviceMode resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementApplicabilityRuleDeviceMode resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceMode|Enumeration|Applicability rule for device mode. Possible values are: `standardConfiguration`, `sModeConfiguration`.|
|name|String|Name for object.|
|ruleType|Enumeration|Applicability Rule type. Possible values are: `include`, `exclude`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
  "deviceMode": "String",
  "name": "String",
  "ruleType": "String"
}
```

