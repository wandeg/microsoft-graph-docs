---
title: "userExperienceAnalyticsDeviceStartupProcessPerformance resource type"
description: "The user experience analytics device startup process performance."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userExperienceAnalyticsDeviceStartupProcessPerformance resource type


Namespace: microsoft.graph

The user experience analytics device startup process performance.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceCount|Int64|User experience analytics device startup process summarized count.|
|id|String|The unique identifier of the user experience analytics device startup process performance.|
|medianImpactInMs|Int32|User experience analytics device startup process median impact in milliseconds.|
|processName|String|User experience analytics device startup process name.|
|productName|String|The user experience analytics device startup process product name.|
|publisher|String|The User experience analytics device startup process publisher.|
|totalImpactInMs|Int32|User experience analytics device startup process total impact in milliseconds.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.management.services.api.userExperienceAnalyticsDeviceStartupProcessPerformance",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.userExperienceAnalyticsDeviceStartupProcessPerformance",
  "id": "String (identifier)",
  "processName": "String",
  "productName": "String",
  "publisher": "String",
  "deviceCount": "Integer",
  "medianImpactInMs": "Integer",
  "totalImpactInMs": "Integer"
}
```

