---
title: "statusDetails resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# statusDetails resource type




Inherits from [statusBase](../resources/statusBase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|additionalDetails|String||
|errorCategory|String||
|errorCode|String||
|reason|String||
|recommendedAction|String||
|status|Enumeration| Inherited from [statusBase](../resources/statusBase.md). Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.statusDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.statusDetails",
  "status": "String",
  "errorCode": "String",
  "reason": "String",
  "additionalDetails": "String",
  "errorCategory": "String",
  "recommendedAction": "String"
}
```

