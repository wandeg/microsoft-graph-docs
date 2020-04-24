---
title: "PrintUsageSummaryByPrinter resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# PrintUsageSummaryByPrinter resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get PrintUsageSummaryByPrinter](../api/printusagesummarybyprinter-get.md)|[PrintUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md)|Read the properties and relationships of a [PrintUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) object.|
|[Update PrintUsageSummaryByPrinter](../api/printusagesummarybyprinter-update.md)|[PrintUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md)|Update the properties of a [PrintUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedBlackAndWhiteJobCount|Int64|**TODO: Add Description**|
|completedColorJobCount|Int64|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|incompleteJobCount|Int64|**TODO: Add Description**|
|printerId|String|**TODO: Add Description**|
|usageDate|Date|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.PrintUsageSummaryByPrinter",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.PrintUsageSummaryByPrinter",
  "id": "String (identifier)",
  "printerId": "String",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": 1024,
  "completedColorJobCount": 1024,
  "incompleteJobCount": 1024
}
```

