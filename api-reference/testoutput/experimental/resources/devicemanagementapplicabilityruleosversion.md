---
title: "deviceManagementApplicabilityRuleOsVersion resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementApplicabilityRuleOsVersion resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|maxOSVersion|String|Max OS version for Applicability Rule.|
|minOSVersion|String|Min OS version for Applicability Rule.|
|name|String|Name for object.|
|ruleType|Enumeration|Applicability Rule type. Possible values are: `include`, `exclude`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
  "minOSVersion": "String",
  "maxOSVersion": "String",
  "name": "String",
  "ruleType": "String"
}
```

