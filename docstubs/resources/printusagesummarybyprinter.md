---
title: "PrintUsageSummaryByPrinter resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# PrintUsageSummaryByPrinter resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get PrintUsageSummaryByPrinter](../api/printusagesummarybyprinter-get.md)|[PrintUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md)|Read properties and relationships of the [PrintUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) object.|
|[Update PrintUsageSummaryByPrinter](../api/printusagesummarybyprinter-update.md)|[PrintUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md)|Update the properties of a [PrintUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedBlackAndWhiteJobCount|Int64||
|completedColorJobCount|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|incompleteJobCount|Int64||
|printerId|String||
|usageDate|Date||

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

