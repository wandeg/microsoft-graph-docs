---
title: "failureInfo resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# failureInfo resource type


Namespace: microsoft.graph.callRecords

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|reason|String|**TODO: Add Description**|
|stage|failureStage|**TODO: Add Description**. Possible values are: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecords.failureInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecords.failureInfo",
  "stage": "String",
  "reason": "String"
}
```

