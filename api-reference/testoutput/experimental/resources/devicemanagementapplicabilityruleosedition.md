---
title: "deviceManagementApplicabilityRuleOsEdition resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagementApplicabilityRuleOsEdition resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|name|String|Name for object.|
|osEditionTypes|Enumeration collection|Applicability rule OS edition type.|
|ruleType|Enumeration|Applicability Rule type. Possible values are: `include`, `exclude`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
  "osEditionTypes": [
    "String"
  ],
  "name": "String",
  "ruleType": "String"
}
```

