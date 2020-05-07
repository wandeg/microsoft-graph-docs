---
title: "deviceManagementApplicabilityRuleDeviceMode resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementApplicabilityRuleDeviceMode resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceMode|windows10DeviceModeType|**TODO: Add Description**. Possible values are: `standardConfiguration`, `sModeConfiguration`.|
|name|String|**TODO: Add Description**|
|ruleType|deviceManagementApplicabilityRuleType|**TODO: Add Description**. Possible values are: `include`, `exclude`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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

