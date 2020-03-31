---
title: "PrintUsageSummaryByUser resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# PrintUsageSummaryByUser resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get PrintUsageSummaryByUser](../api/printusagesummarybyuser-get.md)|[PrintUsageSummaryByUser](../resources/printusagesummarybyuser.md)|Read properties and relationships of the [PrintUsageSummaryByUser](../resources/printusagesummarybyuser.md) object.|
|[Update PrintUsageSummaryByUser](../api/printusagesummarybyuser-update.md)|[PrintUsageSummaryByUser](../resources/printusagesummarybyuser.md)|Update the properties of a [PrintUsageSummaryByUser](../resources/printusagesummarybyuser.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedBlackAndWhiteJobCount|Int64||
|completedColorJobCount|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|incompleteJobCount|Int64||
|usageDate|Date||
|userPrincipalName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.PrintUsageSummaryByUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.PrintUsageSummaryByUser",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": 1024,
  "completedColorJobCount": 1024,
  "incompleteJobCount": 1024
}
```

