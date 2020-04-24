---
title: "PrintUsageSummaryByUser resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# PrintUsageSummaryByUser resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get PrintUsageSummaryByUser](../api/printusagesummarybyuser-get.md)|[PrintUsageSummaryByUser](../resources/printusagesummarybyuser.md)|Read the properties and relationships of a [PrintUsageSummaryByUser](../resources/printusagesummarybyuser.md) object.|
|[Update PrintUsageSummaryByUser](../api/printusagesummarybyuser-update.md)|[PrintUsageSummaryByUser](../resources/printusagesummarybyuser.md)|Update the properties of a [PrintUsageSummaryByUser](../resources/printusagesummarybyuser.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedBlackAndWhiteJobCount|Int64|**TODO: Add Description**|
|completedColorJobCount|Int64|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|incompleteJobCount|Int64|**TODO: Add Description**|
|usageDate|Date|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

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

